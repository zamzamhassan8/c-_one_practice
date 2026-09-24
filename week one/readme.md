Discourse Chapter 1

Week 1 – C# Windows Forms & Variables Practice

Overview

This practice demonstrates how to:

- Create and assign string and integer variables from user inputs.
- Parse string values into integer types using "int.Parse()".
- Clear TextBox and Label controls using ".Clear()", "string.Empty", and """".
- Reset form fields using button event handlers.

---

1. Assigning Date Input Variables

In this step, string variables are assigned directly from the text values entered into the date input controls.

- "Day_of_the_week" – stores input from "txtdayoftheweek".
- "Name_of_the_month" – stores input from "txtdayofthemonth".
- "Numeric_of_the_month" – stores input from "txtdayofthenumeric".
- "day_of_the_year" – stores input from "txtyear".

// Assign variables to use input
Day_of_the_week = txtdayoftheweek.Text;
Name_of_the_month = txtdayofthemonth.Text;
Numeric_of_the_month = txtdayofthenumeric.Text;
day_of_the_year = txtyear.Text;

---

2. Clearing Student Form Controls

In this step, the button click event resets all input fields for the student form using the ".Clear()" method and empties the label text using "string.Empty".

private void bttclear_Click(object sender, EventArgs e)
{
    txtname.Clear();
    txtstudentid.Clear();
    txtdepartment.Clear();
    txtsemester.Clear();
    lblshowinfo.Text = string.Empty;
}

---

3. Student Input Variables and Parsing

In this step, variables are declared and user inputs are captured from the TextBoxes. String values are converted into integers using "int.Parse()".

- "name" – stores the student's name.
- "studentid" – converts and stores the student ID as an integer.
- "department" – stores the student's department.
- "semester" – converts and stores the semester number as an integer.

// Step 1
string name, department, fullInfo;

name = txtname.Text;
int studentid = int.Parse(txtstudentid.Text);
department = txtdepartment.Text;
int semester = int.Parse(txtsemester.Text);

---

4. Clearing Date Form TextBoxes and Labels

In this step, the Clear button event resets all date TextBoxes and clears the output label by assigning an empty string """".

private void bbtClear_Click(object sender, EventArgs e)
{
    // Clear TextBoxes and Label

    // Clearing TextBoxes
    txtdayofthemonth.Text = "";
    txtdayoftheweek.Text = "";
    txtdayofthenumeric.Text = "";
    txtyear.Text = "";

    // Clearing Label
    lbldaoutput.Text = "";
}

---

Conclusion

This practice demonstrates basic C# Windows Forms concepts, including variables, user input, integer parsing, TextBox controls, Label controls, and button click event handlers.