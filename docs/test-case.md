## Authentication Decision Table

| Check   | Condition           | Username          | Password           | Expected Result                                               | Actual Result | Status |
| ------- | ------------------- | ----------------- | ------------------ | ------------------------------------------------------------- | ------------- | ------ |
| AUTH-01 | Blank username      |                   | `secret_sauce`     | `Username is required`                                        |`Username is required`|`Pass`|
| AUTH-02 | Blank password      | `standard_user`   |                    | `Password is required`                                        |`Password is required`|`Pass`|
| AUTH-03 | Invalid credentials | `invalid_user`    | `invalid_password` | `Username and password do not match any user in this service` |`password do not match any user in this service`|`Pass`|
| AUTH-04 | Locked account      | `locked_out_user` | `secret_sauce`     | `Sorry, this user has been locked out`                        |`Sorry, this user has been locked out`|`Pass`|
