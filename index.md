Here is the complete code and structure for your assignment (Assignment 4.3 — Student Marks Table).

Save the code below into a file named marksheet.html. It fulfills all your requirements: data for 5 students across 3 subjects, clean semantic table sections (<thead>, <tbody>, <tfoot>), a descriptive <caption>, meaningful headers, and the use of both colspan and rowspan for professional formatting.

File: marksheet.html
HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Marksheet Table</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f6f9;
            margin: 0;
            padding: 2rem;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }
        .table-container {
            background: #ffffff;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
            width: 100%;
            max-width: 900px;
            overflow-x: auto;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            text-align: left;
            font-size: 0.95rem;
        }
        caption {
            font-size: 1.5rem;
            font-weight: bold;
            color: #2c3e50;
            margin-bottom: 1.5rem;
            text-align: center;
        }
        thead th {
            background-color: #2563eb;
            color: white;
            padding: 0.75rem 1rem;
            text-align: center;
            border: 1px solid #1d4ed8;
        }
        tbody td, tfoot td {
            padding: 0.75rem 1rem;
            border: 1px solid #cbd5e1;
            text-align: center;
        }
        tbody tr:nth-child(even) {
            background-color: #f8fafc;
        }
        tbody tr:hover {
            background-color: #f1f5f9;
        }
        tbody td:nth-child(2) {
            text-align: left; /* Align student names to the left */
        }
        tfoot {
            font-weight: bold;
            background-color: #e2e8f0;
            color: #1e293b;
        }
    </style>
</head>
<body>

    <div class="table-container">
        <table>
            <!-- 4. Table Caption / Title -->
            <caption>Spring Semester 2026 — Student Academic Marksheet</caption>
            
            <!-- 3. Table Header Section -->
            <thead>
                <tr>
                    <!-- 6. Using rowspan for vertical header grouping -->
                    <th rowspan="2">Roll No</th>
                    <th rowspan="2">Student Name</th>
                    <!-- 6. Using colspan for horizontal subject grouping -->
                    <th colspan="3">Subjects (Max Marks: 100)</th>
                    <th rowspan="2">Total Marks</th>
                    <th rowspan="2">Percentage (%)</th>
                </tr>
                <tr>
                    <!-- 7. Meaningful Subject Headers -->
                    <th>Mathematics</th>
                    <th>Science</th>
                    <th>English</th>
                </tr>
            </thead>

            <!-- 3. Table Body Section with 5 Students and 3 Subjects -->
            <tbody>
                <tr>
                    <td>101</td>
                    <td>John Doe</td>
                    <td>85</td>
                    <td>90</td>
                    <td>78</td>
                    <td>253</td>
                    <td>84.33%</td>
                </tr>
                <tr>
                    <td>102</td>
                    <td>Jane Smith</td>
                    <td>92</td>
                    <td>88</td>
                    <td>95</td>
                    <td>275</td>
                    <td>91.67%</td>
                </tr>
                <tr>
                    <td>103</td>
                    <td>Robert Johnson</td>
                    <td>74</td>
                    <td>80</td>
                    <td>82</td>
                    <td>236</td>
                    <td>78.67%</td>
                </tr>
                <tr>
                    <td>104</td>
                    <td>Emily Davis</td>
                    <td>95</td>
                    <td>92</td>
                    <td>96</td>
                    <td>283</td>
                    <td>94.33%</td>
                </tr>
                <tr>
                    <td>105</td>
                    <td>Michael Brown</td>
                    <td>68</td>
                    <td>75</td>
                    <td>70</td>
                    <td>213</td>
                    <td>71.00%</td>
                </tr>
            </tbody>

            <!-- 3 & 5. Table Footer Section showing Averages using colspan -->
            <tfoot>
                <tr>
                    <!-- Using colspan to span across Roll No and Student Name columns -->
                    <td colspan="2" style="text-align: right;">Class Subject Averages:</td>
                    <td>82.8</td>
                    <td>85.0</td>
                    <td>84.2</td>
                    <td colspan="2" style="text-align: center;">Overall Average: 84.0%</td>
                </tr>
            </tfoot>
        </table>
    </div>

</body>
</html>
How to Complete Your Submission:
Save the File: Save the code above as marksheet.html on your computer.

Test in Browser: Double-click the file to open it in your web browser. Check that:

The table displays 5 student rows and 3 subject columns properly.

Header groupings (rowspan and colspan) and footer summary rows render accurately.

Take a Screenshot: Capture a clean browser screenshot of the rendered student marksheet table.

Submit: Turn in your marksheet.html file and the screenshot as required by your assignment instructions!