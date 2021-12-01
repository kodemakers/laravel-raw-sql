| laravel-code      | SQL- QUERIES |
| ----------- | ----------- |
| `One-to-One` <br /> hasOne(UserWallet::class) <br/> $user->wallet() | select * from `user_wallets` <br/> where `user_wallets`.`user_id` = ? <br/> and `user_wallets`.`user_id` is not null |
| `One-to-Many` <br /> hasMany(Notification::class) <br/> $user->notifications() | select * from `notifications` <br/> where `notifications`.`user_id` = ? <br/> and `notifications`.`user_id` is not null |
