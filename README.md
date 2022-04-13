<div class="container">
<div class="row text-center">
<div class="col-12">
# JQuery Datables in .NET Core with Export
</div>
<div class="col-12">
.NET Core v3.1

Bootstrap v4.5.0

jQuery v1.12.4

Datatables v1.10.19
</div>

# Demo
<div class="row text-left">
<div class="col-12 mb-2">
#### Adding/Eiting an employee
![Home Image](https://i.ibb.co/bsvbBMc/Home-JQuery-Datables-Net-Core.gif)</div>

<div class="col-12 mb-2">

#### Datatable

![Home Image](https://i.ibb.co/XXKgB0t/Home.jpg)</div>

<div class="col-12 mb-2">

#### Add Employee

![Home Image](https://i.ibb.co/yY72n8s/Add-Employee.jpg)</div>

<div class="col-12 mb-2">

#### PDF Export

![Home Image](https://i.ibb.co/NsDY0nV/Pdf-Export.jpg)</div>

<div class="col-12 mb-2">

#### Excel Export

![Home Image](https://i.ibb.co/kyXNhHp/Excel-Export.jpg)</div>

</div>

# Setting Up

<div class="row text-left">

<div class="col-12 mb-4">

#### App Settings

Go to the project root directory and set the connection string in appsettins.json file.

You need to set the "Server" and the "Database". ![Cinque Terre](https://i.ibb.co/1b234XK/connection-string.jpg)

You can read more on connection strings [here](https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-mvc-app/working-with-sql?view=aspnetcore-3.1&tabs=visual-studio)

</div>

<div class="col-12 mb-4">

#### Exporting Database

Create a database in SQL Server with the same name as that in the connectiion string. E.g. "EmployeeDB" ![](https://i.ibb.co/mhmzd8J/employee-db-sql.jpg)

Open the solution file in Visual Studio and click the Package Manager Console at the bottom, or on top, click on Tools, then NuGet Package Manager, then Package Manager Console.

Then run the following commands:

*   Add-Migration "Initial Migration"
*   Update-Database

That's all. You can now run the application. Click on the Run/IIS Express button in Visual studio to launch the application.

<button type="button" class="btn btn-primary" data-toggle="collapse" data-target="#demo">Sample Employee Script</button>

<div id="demo" class="collapse rounded bg-dark text-warning p-3 mt-2">INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'01a3df2f-e8a4-4562-ba53-d2e9cf1751a8', N'Michael', N'Bruce', N'Javascript Developer ', N'Singapore', CAST(N'1985-03-03' AS Date), CAST(N'2020-10-21' AS Date), N'183000', CAST(N'2020-09-12T07:10:10.0682893' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'16eda51b-ee5b-4bcd-b414-9af85364014e ', N'Donna ', N'Snider', N'Customer Support ', N'Hamburg', CAST(N'2001-03-03' AS Date), CAST(N'2020-10-05' AS Date), N'112000', CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'19778c2a-e0b1-47ea-881d-fdd6da7b548f', N'Charde', N'Marshall', N'Regional Director', N'San Francisco ', CAST(N'1988-10-14' AS Date), CAST(N'2022-06-16' AS Date), N'470000', CAST(N'2020-09-12T07:10:10.0682893' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'19f8740f-7e6f-4be3-91d4-bfaf4f669557', N'Ablie', N'Kassama', N'Lead Developer', N'Hamburg', CAST(N'1991-10-19' AS Date), CAST(N'2021-04-01' AS Date), N'495000', CAST(N'2020-09-12T08:02:27.1783052' AS DateTime2), CAST(N'2020-09-12T08:02:19.4933588' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'1bc4b7ba-e90a-42f8-8b08-2635347820a2', N'Sakura ', N'Yamamoto', N'Support Engineer', N'Tokyo', CAST(N'1999-03-26' AS Date), CAST(N'2020-11-12' AS Date), N'149000', CAST(N'2020-09-12T07:10:10.0682893' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'1f1eb668-11f0-4b7d-abd8-083ef75bf8b7', N'Yuri ', N'Berry ', N'Chief Marketing Officer (CMO) ', N'London', CAST(N'1992-02-08' AS Date), CAST(N'2020-10-08' AS Date), N'675000', CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'4b389df1-da38-4d67-b87d-acdce7a780b0', N'Brenden ', N'Wagner', N'Software Engineer ', N'New York', CAST(N'1992-12-16' AS Date), CAST(N'2020-09-21' AS Date), N'206850', CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'863bacb6-6466-486b-a5c4-f79268d7456d ', N'Cedric ', N'Kelly', N'Senior Javascript Developer ', N'Edinburgh', CAST(N'1996-02-10' AS Date), CAST(N'2019-03-29' AS Date), N'433060', CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'8e4bebd0-0a69-4fc9-9146-4e14089eb255 ', N'Vivian ', N'Harrell', N'Financial Controller ', N'San Francisco ', CAST(N'1999-11-15' AS Date), CAST(N'2020-10-15' AS Date), N'367222', CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'c0812b5b-f28e-41ea-bad6-8ea5bfbec448', N'Doris ', N'Wilder', N'Sales Assistant', N'Sydney', CAST(N'1990-07-17' AS Date), CAST(N'2020-10-22' AS Date), N'185600', CAST(N'2020-09-12T07:10:10.0682893' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'd162f111-c586-4908-915a-586ca01d311b', N'Ousman', N'Kassama', N'Branch Manager', N'Kairaba Avenue', CAST(N'1988-10-14' AS Date), CAST(N'2022-06-16' AS Date), N'620000', CAST(N'2020-09-12T07:10:10.0682893' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))  

INSERT [dbo].[Employee] ([EmployeeID], [FirstName], [LastName], [Position], [OfficeLocation], [DateOfBirth], [StartDate], [Salary], [UpdateDate], [DateAdded]) VALUES (N'd162f111-c586-4908-915a-586ca91d311b', N'Jackson', N'Bradshaw', N'Director', N'New York ', CAST(N'1988-10-14' AS Date), CAST(N'2022-06-16' AS Date), N'645750', CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2), CAST(N'2020-09-12T07:10:10.0683452' AS DateTime2))</div>

#

The demo sql script couls also be found in wwwroot/sql/Employee.sql.

</div>

<div class="col-12 mb-4">

#### Application Structure & Resources

The application uses Bootstrap v4.5.0, Datatables v1.10.19, and JQuery v1.12.4.

Customization of the export button styling is done in the site css file located in wwwroot/css/site.css. ![](https://i.ibb.co/mTDj4wJ/cuztomize-buttons.jpg)

You set set the export buttons you wnat to be visible in the site js file located in wwwroot/js/site-footer.js. ![](https://i.ibb.co/0K3Pjbs/column-visibility.jpg)

The "columns: [0, 1, 2, 3, 4, 5, 6]" is use to set the visible columns for the event.

The "Action" modal items are set in the site-header js file located in wwwroot/js/site-header.js.

They are based on click event handlers, whhich retrieves the value in the "data-" attribute ![](https://i.ibb.co/0XK4XQQ/modal-setters-all.jpg)

</div>

<div class="col-12 mb-4">

#### App Helpers

The app helpers are located in App_Code/AppHelpers.cs

Below are the helpers and theier functions:

*   GetAge(DateTime date_of_birth) => Generates employee age from date of birth
*   InpuDateFormat(DateTime input_date) => Convert date to yyyy-MM-dd format
*   FormatSalary(string number) => Formats the number adding a comma per every thousand

</div>

</div>

</div>
