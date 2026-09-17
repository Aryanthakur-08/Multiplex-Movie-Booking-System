# Multiplex Movie Booking System

## Overview
The **Multiplex Movie Booking System** is a robust, console-based Java application that simulates the experience of booking movie tickets in a modern multiplex. It provides two distinct portals: a User Portal for browsing movies, selecting seats via a visual seat map, ordering snacks, and booking tickets; and an Admin Portal for managing the movie catalogue, scheduling shows, and viewing real-time revenue analytics.

## Features
### User Portal
*   **Browse Movies & Shows**: View currently playing movies and their scheduled timings across different screens.
*   **Visual Seat Selection**: Interactive tiered seating layout (VIP, Premium, Executive, Normal) with real-time availability tracking.
*   **Snack Bar**: Order add-on snacks (Popcorn, Nachos, Beverages) during the booking process.
*   **Promo Codes**: Apply permanent discount codes (e.g., WELCOME10) or earn single-use bulk reward codes for booking 5+ seats.
*   **Detailed Billing**: Automatic calculation of seat totals, snack totals, discounts, 18% GST, and convenience fees.
*   **Ticket Wallet & Cancellation**: View active tickets in your wallet or cancel them for a full refund (which frees up the seats and revokes promo codes).

### Admin Portal
*   **Revenue Analytics**: View per-movie, per-show ticket sales and revenue generation, along with grand platform totals.
*   **Catalogue Management**: Add new movies or schedule new shows on specific screens.
*   **Cascade Deletion**: Removing a movie automatically deletes its scheduled shows and revokes all booked tickets for those shows.

## Technologies/Tools Used
*   **Language**: Java 17 (JDK 17+)
*   **Concepts Used**: Object-Oriented Programming (OOP), Collections Framework (List, Set, Map), Enums, Lambda Expressions, Stream API, UUID generation.
*   **Architecture**: Layered design with distinct Separation of Concerns (Presentation, Business Logic, and Model/Data).
*   **Data Storage**: In-memory collections (HashMap, ArrayList) for zero-dependency execution.

## Steps to Install & Run the Project
1.  **Prerequisites**: Ensure you have Java (JDK 17 or higher) installed on your system. You can verify this by running `java -version` in your terminal.
2.  **Navigate to Source**: Open your terminal/command prompt and navigate to the `src` directory containing `MultiplexBookingSystem.java`.
    ```bash
    cd MovieBookingSystem/src
    ```
3.  **Compile the Code**:
    ```bash
    javac MultiplexBookingSystem.java
    ```
4.  **Run the Application**:
    ```bash
    java MultiplexBookingSystem
    ```

## Instructions for Testing
You can manually test the system using the following test cases:

1.  **User Booking Flow**:
    *   Select `1` to Login as User.
    *   Select `1` to Book Tickets.
    *   Choose a Movie ID (e.g., `M04` for Dune) and a Show ID.
    *   Select seats from the visual map (e.g., `A1 A2` for VIP seats).
    *   Add snacks if prompted, then apply the promo code `WELCOME10`.
    *   Verify the final invoice calculations (including GST).
2.  **Ticket Cancellation**:
    *   From the User Dashboard, select `3` to Cancel a Ticket.
    *   Enter the Ticket ID provided in the previous step.
    *   Verify that the refund is processed.
3.  **Admin Analytics**:
    *   Select `2` to Login as Admin.
    *   Select `1` to View Analytics.
    *   Verify that the revenue reflects any tickets you just booked.

## Screenshots
Please refer to the `Multiplex_Movie_Booking_System_Report.docx` file included in this repository for comprehensive, high-resolution screenshots of the terminal interface, including:
*   Main Menu & User Dashboard
*   Movie Catalogue & Visual Seat Map
*   Snack Bar Integration & Detailed Invoice Receipt
*   Admin Analytics Dashboard
