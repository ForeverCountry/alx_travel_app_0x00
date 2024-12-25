# ALX Travel App

## Milestone 2: Creating Models, Serializers, and Seeders

### Objective
Define the database models, create serializers for API data representation, and implement a management command to seed the database.

---

### Instructions

#### 1. Duplicate Project
- Duplicate the project `alx_travel_app` to `alx_travel_app_0x00`.

#### 2. Create Models
- In `listings/models.py`, define the following models:
  - **Listing**: Represents properties available for booking.
  - **Booking**: Tracks reservations for listings.
  - **Review**: Stores user reviews for listings.
- Ensure each model has:
  - Appropriate fields.
  - Proper relationships (e.g., foreign keys).
  - Relevant constraints (e.g., `null=False`, unique identifiers).

#### 3. Set Up Serializers
- In `listings/serializers.py`:
  - Create serializers for the **Listing** and **Booking** models.
  - Ensure the serializers handle API data representation effectively.

#### 4. Implement Seeders
- Create a custom management command to populate the database with sample data:
  - Location: `listings/management/commands/seed.py`.
  - Populate the database with sample `Listing`, `Booking`, and `Review` data.

#### 5. Run Seed Command
- Test the seeder script to confirm the database is populated correctly.
- Use the following command:
  ```bash
  python manage.py seed
  ```
