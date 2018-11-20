# sprint2-vos

1. Add the files included in this repository to the appropriate folders in your project folder.

2. The `volorgs` table (in your case, it may be the `vos` table) was seeded with dummy data using the Faker library.
To install this library, run the following command in your Terminal/cmd:
> `composer require fzaninotto/faker`  

The volunteers table was also seeded with dummy data, however, if you already have records in your `volunteers` table, you do not need to seed the database.

To seed the databases, run the following commands:
> `composer dump-autoload`

> `php artisan db:seed --class=VolorgTableSeeder`

> `php artisan db:seed --class=VolunteersTableSeeder` 

###### If your `vos` table already has records and you prefer not to install the Faker library, you may do so, but you may need to do a mass search and replace in the files, replacing `volorgs` with `vos` and `volorg` with `vo`. However, to avoid any possible issues (which I may not be able to help you with 🙃), I suggest that you either rename your `vos` table to `volorgs` or create a new `volorgs` table altogether.

### For logging in a VO, the default password is set to `123456`
