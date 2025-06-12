# Project Plan: NimbusCloud

**Description:** A simple web hosting platform built with Ruby on Rails, offering basic domain management features.


## Development Goals

- [ ] Configure the tailwindcss-rails gem by running `rails tailwindcss:install` and configuring the asset pipeline.
- [ ] Add model validations to the Domain model (app/models/domain.rb) to ensure name is present and the plan is restricted to a predefined set of options (e.g., 'basic', 'premium', 'enterprise').
- [ ] Customize the domains scaffold views (app/views/domains/) to apply Tailwind CSS classes to improve the user interface, focusing on responsiveness and aesthetics.
- [ ] Modify the DomainsController (app/controllers/domains_controller.rb) to associate domains with the currently logged-in user. Ensure only the user who created the domain can edit or delete it. Implement `before_action :authenticate_user!` and a `before_action :correct_user, only: [:edit, :update, :destroy]` method.
- [ ] Implement user authentication and authorization using Devise. Configure Devise routes and views to provide a user-friendly login and registration experience.
- [ ] Add a user profile page where users can view their registered domains.
- [ ] Add a helper method to display the user's name or email on the layout.
- [ ] In the application layout (app/views/layouts/application.html.erb), add navigation links for 'My Domains', 'Profile', and 'Sign Out' based on whether a user is signed in.
- [ ] Add a 'status' field to the Domain model and update the scaffold to allow users to change the domain status (e.g., 'active', 'inactive', 'pending').
- [ ] Secure the application against common web vulnerabilities such as Cross-Site Scripting (XSS) and Cross-Site Request Forgery (CSRF) by using appropriate Rails features and security best practices.
