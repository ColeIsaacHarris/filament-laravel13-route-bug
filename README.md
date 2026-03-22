## Steps to Reproduce Issue:

- Create a user with php artisan filament:new-user
- Start local web server using: 'php artisan serve'
- Visit admin.localhost and attempt to log in
- Expected: Dashboard loads after login Actual: Route [filament.admin.pages.dashboard] not defined

This does not occur on panels without ->domain(), because non-domain routes still use direct assignment.
