By Roker2

## fingerprint.goodix.so

Need to change to CMP X2, X1 or CMP X1, X0

CMP X2, X1 = 5F 00 01 EB in HEX

CMP X1, X0 = 3F 00 00 EB in HEX

Based on comparing Leeco S2 blobs

Maybe need to patch Aliplay functions

| Function                           | Patch place | Patch status (patched or not) | New command |
| :--------------------------------- | :---------- | :---------------------------- | :---------- |
| goodix_sensor_fp_enroll            | C3F0        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C3F4        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C3F8        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C3FC        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C404        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_clear_enroll_env  | C548        | yes                           | CMP X1, X0  |
| goodix_sensor_fp_clear_enroll_env  | C54C        | yes                           | CMP X1, X0  |
| goodix_sensor_fp_clear_enroll_env  | C550        | yes                           | CMP X1, X0  |
| goodix_sensor_fp_clear_enroll_env  | C558        | yes                           | CMP X1, X0  |
| goodix_sensor_fp_set_session_id    | C644        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C648        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C64C        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C650        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C658        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_match             | C770        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_match             | C774        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_match             | C778        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_match             | C77C        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_match             | C784        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C8EC        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C8F0        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C8F4        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C8F8        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C900        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_save              | C9DC        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_save              | C9E0        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_save              | C9E4        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_save              | C9E8        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_save              | C9F0        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | CB0C        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | CB10        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | CB14        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | CB1C        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_remove            | CD5C        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_remove            | CD60        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_remove            | CD64        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_remove            | CD68        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_remove            | CD70        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CFB0        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CFB4        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CFB8        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CFBC        | yes                           | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CFC4        | yes                           | CMP X2, X1  |
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
| goodix_sensor_fp_enroll_verify     | C2EC        | no                            | CMP X2, X1  |
| goodix_sensor_fp_enroll_verify     | C2F0        | no                            | CMP X2, X1  |
| goodix_sensor_fp_enroll_verify     | C2F4        | no                            | CMP X2, X1  |
| goodix_sensor_fp_enroll_verify     | C2F8        | no                            | CMP X2, X1  |
| goodix_sensor_fp_enroll_verify     | C300        | no                            | CMP X2, X1  |
| goodix_sensor_fp_set_user_id       | C200        | no                            | CMP X2, X1  |
| goodix_sensor_fp_set_user_id       | C204        | no                            | CMP X2, X1  |
| goodix_sensor_fp_set_user_id       | C208        | no                            | CMP X2, X1  |
| goodix_sensor_fp_set_user_id       | C20C        | no                            | CMP X2, X1  |
| goodix_sensor_fp_set_user_id       | C214        | no                            | CMP X2, X1  |
| goodix_enable_screen_lock          | D1C0        | no                            | CMP X2, X1  |
| goodix_enable_screen_lock          | D1C4        | no                            | CMP X2, X1  |
| goodix_enable_screen_lock          | D1C8        | no                            | CMP X2, X1  |
| goodix_enable_screen_lock          | D1CC        | no                            | CMP X2, X1  |
| goodix_enable_screen_lock          | D1D4        | no                            | CMP X2, X1  |
| goodix_disable_screen_lock         | D29C        | no                            | CMP X2, X1  |
| goodix_disable_screen_lock         | D2A0        | no                            | CMP X2, X1  |
| goodix_disable_screen_lock         | D2A4        | no                            | CMP X2, X1  |
| goodix_disable_screen_lock         | D2A8        | no                            | CMP X2, X1  |
| goodix_disable_screen_lock         | D2B0        | no                            | CMP X2, X1  |

12 functions, 58 patch places