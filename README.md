Work In Progress For Santoni


By Roker2

## fingerprint.goodix.so

Need to change to CMP X2, X1 or CMP X1, X0

CMP X2, X1 = 5F 00 01 EB in HEX

CMP X1, X0 = 3F 00 00 EB in HEX

Based on comparing Leeco S2 blobs

Maybe need to patch Aliplay functions

| Function                           | Patch place | Patch status (patched or not) | New command |
| :--------------------------------- | :---------- | :---------------------------- | :---------- |
| goodix_sensor_fp_enroll            | C0EC        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C0F0        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C0F4        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C0F8        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C100        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_clear_enroll_env  | C244        | yes                           | CMP X1, X0  |
| goodix_sensor_fp_clear_enroll_env  | C248        | yes                           | CMP X1, X0  |
| goodix_sensor_fp_clear_enroll_env  | C24C        | yes                           | CMP X1, X0  |
| goodix_sensor_fp_clear_enroll_env  | C254        | yes                           | CMP X1, X0  |
| goodix_sensor_fp_set_session_id    | C340        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C344        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C348        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C34C        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C354        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_match             | C454        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_match             | C458        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_match             | C45C        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_match             | C460        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_match             | C468        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C5C4        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C5C8        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C5CC        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C5D0        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C5D8        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_save              | C6B4        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_save              | C6B8        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_save              | C6BC        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_save              | C6C0        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_save              | C6C8        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | C7E4        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | C7E8        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | C7EC        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | C7F4        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_remove            | C9FC        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_remove            | CA00        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_remove            | CA04        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_remove            | CA08        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_remove            | CA10        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CB5C        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CB60        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CB64        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CB68        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CB70        | yes                           | CMP X2, X1  |
| goodix_sensor_init                 | BA58        | yes                           | CMP X2, X1  |
| goodix_sensor_init                 | BA5C        | yes                           | CMP X2, X1  |
| goodix_sensor_init                 | BA60        | yes                           | CMP X2, X1  |
| goodix_sensor_init                 | BA64        | yes                           | CMP X2, X1  |
| goodix_sensor_init                 | BA6C        | yes                           | CMP X2, X1  |
| goodix_sensor_set_active_group     | BEA8        | yes                           | CMP X2, X1  |
| goodix_sensor_set_active_group     | BEAC        | yes                           | CMP X2, X1  |
| goodix_sensor_set_active_group     | BEB0        | yes                           | CMP X2, X1  |
| goodix_sensor_set_active_group     | BEB4        | yes                           | CMP X2, X1  |
| goodix_sensor_set_active_group     | BEBC        | yes                           | CMP X2, X1  |
| goodix_sensor_fill_auth_token_hmac | C0D4        | yes                           | CMP X2, X1  |
| goodix_sensor_fill_auth_token_hmac | C0D8        | yes                           | CMP X2, X1  |
| goodix_sensor_fill_auth_token_hmac | C0DC        | yes                           | CMP X2, X1  |
| goodix_sensor_fill_auth_token_hmac | C0E0        | yes                           | CMP X2, X1  |
| goodix_sensor_fill_auth_token_hmac | C0E8        | yes                           | CMP X2, X1  |

12 functions, 58 patch places
