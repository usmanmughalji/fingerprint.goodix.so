By Roker2

## fingerprint.goodix.so

Need to change to CMP X2, X1 or CMP X1, X0

CMP X2, X1 = 5F 00 01 EB in HEX

CMP X1, X0 = 3F 00 00 EB in HEX

Based on comparing Leeco S2 blobs

Maybe need to patch Aliplay functions

| Function                           | Patch place | Patch status (patched or not) | New command |
| :--------------------------------- | :---------- | :---------------------------- | :---------- |
| goodix_sensor_fp_enroll            | C3F0        | no                            | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C3F4        | no                            | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C3F8        | no                            | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C3FC        | no                            | CMP X2, X1  |
| goodix_sensor_fp_enroll            | C404        | no                            | CMP X2, X1  |
| goodix_sensor_fp_clear_enroll_env  | C548        | no                            | CMP X1, X0  |
| goodix_sensor_fp_clear_enroll_env  | C54C        | no                            | CMP X1, X0  |
| goodix_sensor_fp_clear_enroll_env  | C550        | no                            | CMP X1, X0  |
| goodix_sensor_fp_clear_enroll_env  | C558        | no                            | CMP X1, X0  |
| goodix_sensor_fp_set_session_id    | C644        | no                            | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C648        | no                            | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C64C        | no                            | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C650        | no                            | CMP X2, X1  |
| goodix_sensor_fp_set_session_id    | C658        | no                            | CMP X2, X1  |
| goodix_sensor_fp_match             | C770        | no                            | CMP X2, X1  |
| goodix_sensor_fp_match             | C774        | no                            | CMP X2, X1  |
| goodix_sensor_fp_match             | C778        | no                            | CMP X2, X1  |
| goodix_sensor_fp_match             | C77C        | no                            | CMP X2, X1  |
| goodix_sensor_fp_match             | C784        | no                            | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C8EC        | no                            | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C8F0        | no                            | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C8F4        | no                            | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C8F8        | no                            | CMP X2, X1  |
| goodix_sensor_fp_cancel            | C900        | no                            | CMP X2, X1  |
| goodix_sensor_fp_save              | C9DC        | no                            | CMP X2, X1  |
| goodix_sensor_fp_save              | C9E0        | no                            | CMP X2, X1  |
| goodix_sensor_fp_save              | C9E4        | no                            | CMP X2, X1  |
| goodix_sensor_fp_save              | C9E8        | no                            | CMP X2, X1  |
| goodix_sensor_fp_save              | C9F0        | no                            | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | CB0C        | no                            | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | CB10        | no                            | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | CB14        | no                            | CMP X2, X1  |
| goodix_sensor_fp_get_fp_list       | CB1C        | no                            | CMP X2, X1  |
| goodix_sensor_fp_remove            | CD5C        | no                            | CMP X2, X1  |
| goodix_sensor_fp_remove            | CD60        | no                            | CMP X2, X1  |
| goodix_sensor_fp_remove            | CD64        | no                            | CMP X2, X1  |
| goodix_sensor_fp_remove            | CD68        | no                            | CMP X2, X1  |
| goodix_sensor_fp_remove            | CD70        | no                            | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CFB0        | no                            | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CFB4        | no                            | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CFB8        | no                            | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CFBC        | no                            | CMP X2, X1  |
| goodix_sensor_fp_gxCmd             | CFC4        | no                            | CMP X2, X1  |
| goodix_sensor_init                 | BA58        | no                            | CMP X2, X1  |
| goodix_sensor_init                 | BA5C        | no                            | CMP X2, X1  |
| goodix_sensor_init                 | BA60        | no                            | CMP X2, X1  |
| goodix_sensor_init                 | BA64        | no                            | CMP X2, X1  |
| goodix_sensor_init                 | BA6C        | no                            | CMP X2, X1  |
| goodix_sensor_set_active_group     | BEA8        | no                            | CMP X2, X1  |
| goodix_sensor_set_active_group     | BEAC        | no                            | CMP X2, X1  |
| goodix_sensor_set_active_group     | BEB0        | no                            | CMP X2, X1  |
| goodix_sensor_set_active_group     | BEB4        | no                            | CMP X2, X1  |
| goodix_sensor_set_active_group     | BEBC        | no                            | CMP X2, X1  |
| goodix_sensor_fill_auth_token_hmac | C0D4        | no                            | CMP X2, X1  |
| goodix_sensor_fill_auth_token_hmac | C0D8        | no                            | CMP X2, X1  |
| goodix_sensor_fill_auth_token_hmac | C0DC        | no                            | CMP X2, X1  |
| goodix_sensor_fill_auth_token_hmac | C0E0        | no                            | CMP X2, X1  |
| goodix_sensor_fill_auth_token_hmac | C0E8        | no                            | CMP X2, X1  |

12 functions, 58 patch places