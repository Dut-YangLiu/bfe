# Condition Primitive Standard

- **Request** or **Response**
  - Condition primitive about request is used ”**req_**“ prefix
    - e.g. **req_host_in()**
  - Condition primitive about response is used ”**res_**“ prefix
    - e.g. **res_code_in()**
  - Condition primitive about session is used ”**ses_**“ prefix
    - e.g. **ses_vip_in()**
  - Condition primitive about system is used ”**bfe_**“ prefix
    - e.g. **bfe_time_range**()
- Compare actions include as follows:
  - **match**：accurate matching
    - In this situation, the only one parameter is given
  - **in**：if the value is in the configured set
  - **prefix_in**：if the value prefix is in the configured set
  - **suffix_in**：if the value suffix is in the configured set
  - **key_exist**：if the key exists
    - In general, this action is used in the compare of query/cookie/header
  - **value_in**：for the configured key, judge if the value is in the configured value set
  - **value_prefix_in**：for the configured key, judge if the value prefix is in the configured set
  - **value_suffix_in**：for the configured key, judge if the value suffix is in the configured set
  - **range**: scope match
    - In general, this action is used in the compare of ip/time
  - **regmatch**：regular match
    - This action is not encouraged to use
  - **dictmatch**：if matching the content of dictionary
  - **contain**: if include the configured string