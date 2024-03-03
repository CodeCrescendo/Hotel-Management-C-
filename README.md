# Hotel-Management-C-
It uses the different OS concepts such as Linux commands, process creation, inter-process communication (shared memory and pipes) to create a hotel management system application. 

The system is designed to simulate the operations of a hotel environment using processes as representations of various entities within the hotel. These entities include:

1. Admin: Oversees the overall functioning of the system.
2. Hotel Manager: Responsible for managing hotel operations, including overseeing earnings and handling termination requests.
3. Tables: Represented as processes, each representing a table within the hotel. The system can handle a maximum of 10 concurrent table processes.
4. Customers: Represented as child processes of table processes, each customer process represents a customer sitting at a particular table.
5. Waiters: Also represented as processes, with each waiter assigned to a specific table. Waiters take orders from customers at their assigned table and calculate the total bill amount for that table. Each waiter is associated with a unique Waiter ID.
6. Menu: A predefined menu from which customers can order food items.

Key points about the system's functionality:

- Each table process can create one or more customer processes, with a maximum of five concurrent customer processes per table.
- The number of table processes is equal to the number of waiter processes, and each waiter attends to a specific table based on its number.
- Table and waiter processes do not have a parent-child relationship, meaning they operate independently.
- During execution, each table process should run in a separate terminal, as should each waiter process.
- The Hotel Manager process oversees earnings, calculating the total earnings of all waiters, and handles termination requests initiated by the Admin process.

The system's workflow involves customers entering the hotel, sitting at tables, ordering food from the menu, waiters taking orders, calculating bills, and the Hotel Manager overseeing earnings and handling termination requests.

Overall, the system provides a detailed simulation of a hotel environment with multiple interacting processes representing different entities within the hotel.
