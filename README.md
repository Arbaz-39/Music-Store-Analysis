-- Project Overview --
Objective: Analyze data from a music store to gain insights into sales, customer behavior, inventory management, and other key metrics.

-- Key Components --
Data Structure:

Tables Involved:
1. artist: Contains information about music artists (e.g., artist_id, name).
2. album: Information about albums (e.g., album_id, title, artist_id).
3. track: Details of individual tracks (e.g., track_id, name, album_id, media_type_id,genre_id,compoer,milliseconds,bytes,unit_price).
4. customer: Information about customers (e.g., customer_id, first_name,last_name,company,address,city,state,country,postal_code,phone,fax,email,support_rep_id).
5. playlist: Information about the playlist(e.g., playlist_id,name).
6. playlist_track: Information related to playlist track (e.g., playlist_id,track_id).
7. media_type: Information about type of media(e.g., media_type_id,name).
8. genre: Information related to genre of the track(e.g., genre_id,name)
9. invoice: Information related to sales of music and its customers(e.g., invoice_id,customer_id,billing_address, billing_city,billing_state,billing_country, billing_postal_code, total).
10. invoice_line: Information related to particular purchase(e.g., invoice_line_id,invoice_id,track_id, unit_price,quantity).
11. employee: Information related to the employee(e.g., employee_id, first_name, last_name, title, reports_to, birthdate, hire_date, address, city,state, country,postal_code,phone, fax,email).

    
SQL Concepts Used:
1. Subqueries: Using where clause and aggregate function (avg), we found the track names that have a song length longer than the average song length.

2. Joins: To combine data from multiple tables (e.g., joining customer table with invoice table  with to get customer details who spent the most money).
  
3. Common Table Expressions (CTEs): For organizing complex queries, making them easier to read and manage.
   
4. Window Functions: Using row_number, we found the most popular music Genre for each country.

   
-- Analysis Examples --
1. The senior most employee based on job title.

2. The country having the most invoices.

3. The top 3 values of total invoice.

4. The city that has the highest sum of invoice totals.

5. The customer who has spent the most money.

6. Details of all Rock Music listeners.

7. Artist name and total track count of the top 10 rock bands.

8. All the track names that have a song length longer than the average song length.

9.  Amount spent by each customer on artists.

10. The most popular music Genre for each country

