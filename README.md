<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Student Reg Form</title>
</head>
<body>
    <h1>Student Registration Form</h1>
    <form action="welcome.html" method="get" novalidate>
        <fieldset>
            <legend>Personal Information</legend>
            <p>
                <label for="reg_name">Full Name:</label><br />
                <input type="text" id="reg_name" name="reg_name" required pattern="[A-Za-z]{3,50}" autocomplete="off" />
            </p>
            <p>
                <label for="reg_email">Email:</label><br />
                <input type="email" id="reg_email" name="reg_email" pattern="[a-zA-Z]+\.{1}[0-9]{6}@marwadiuniversity\.ac\.in" />
            </p>
            <p>
                <label for="reg_password">Password:</label><br />
                <input type="password" id="reg_password" name="reg_password" pattern="(?=.*[A-Z])(?=.*[a-z])(?=.*\d).{8,}" />
            </p>
            <p>
                <label for="reg_number">Phone number:</label><br />
                <input type="tel" id="reg_number" name="reg_number" pattern="[0-9]{10}" />
            </p>
            <p>
                <label for="reg_age">Age:</label><br />
                <input type="number" id="reg_age" name="reg_age" />
            </p>
            <p>
                <label for="address">Address:</label><br />
                <textarea id="address" name="address" rows="4" cols="50"></textarea>
            </p>
            <p>
                <label>Gender:</label><br />
                <input type="radio" id="gender_male" name="reg_gender" value="Male" checked />
                <label for="gender_male">Male</label>
                <input type="radio" id="gender_female" name="reg_gender" value="Female" />
                <label for="gender_female">Female</label>
            </p>
            <p>
                <label>Hobbies:</label><br />
                <input type="checkbox" id="hobby_cricket" name="hobbies[]" value="Cricket" checked />
                <label for="hobby_cricket">Cricket</label>
                <input type="checkbox" id="hobby_hockey" name="hobbies[]" value="Hockey" />
                <label for="hobby_hockey">Hockey</label>
                <input type="checkbox" id="hobby_nothing" name="hobbies[]" value="Nothing" />
                <label for="hobby_nothing">Nothing</label>
            </p>
        </fieldset>
        <fieldset>
            <legend>Preferences & Extras</legend>
            <p>
                <label for="reg_file">Upload Profile Picture:</label><br />
                <input type="file" id="reg_file" name="reg_file" multiple />
            </p>
            <p>
                <label for="fav_color">Color:</label><br />
                <input type="color" id="fav_color" name="fav_color" />
            </p>
            <p>
                <label for="search_course">Search for Course:</label><br />
                <input type="search" id="search_course" name="search_course" />
            </p>
            <p>
                <label for="course_range">Course Interest Range:</label><br />
                <input type="range" id="course_range" name="course_range" />
            </p>
            <p>
                <label for="reg_website">Personal Website:</label><br />
                <input type="url" id="reg_website" name="reg_website" pattern="https?://.+" />
            </p>
            <p>
                <label for="reg_dept">Course Type: </label><br />
                <select id="reg_dept" name="reg_dept[]" size="5" multiple>
                    <optgroup label="engg">
                        <option value="CE">CE</option>
                        <option value="EE" selected>EE</option>
                        <option value="ME">ME</option>
                        <option value="CIV">CIV</option>
                    </optgroup>
                    <optgroup label="Management">
                        <option value="BBA">BBA</option>
                        <option value="MBA">MBA</option>
                    </optgroup>
                </select>
            </p>
            <p>
                <label for="reg_country">Preferred Country:</label><br />
                <input list="countries" id="reg_country" name="reg_country" />
                <datalist id="countries">
                    <option value="USA">USA</option>
                    <option value="UK">UK</option>
                    <option value="India">India</option>
                    <option value="Japan">Japan</option>
                </datalist>
            </p>
            <p>
                <input type="checkbox" id="reg_agree" name="reg_agree" value="I agree" checked />
                <label for="reg_agree">Agree to Terms</label>
            </p>
        </fieldset>
        <fieldset>
            <legend>Date & Time Info</legend>
            <p>
                <label for="reg_date">Select Date of Birth:</label><br />
                <input type="date" id="reg_date" name="reg_date" />
            </p>
            <p>
                <label for="reg_time">Select Time:</label><br />
                <input type="time" id="reg_time" name="reg_time" />
            </p>
            <p>
                <label for="reg_month">Select Month:</label><br />
                <input type="month" id="reg_month" name="reg_month" />
            </p>
            <p>
                <label for="reg_week">Select Week:</label><br />
                <input type="week" id="reg_week" name="reg_week" />
            </p>
            <p>
                <label for="reg_datetime">Select Date and Time:</label><br />
                <input type="datetime-local" id="reg_datetime" name="reg_datetime" />
            </p>
        </fieldset>
        <fieldset>
            <legend>Form Controls</legend>
            <p>
                <button type="button" onclick="sub()">Click Me</button>
                <input type="image" src="butterfly.png" alt="Register Now" height="50" width="50" />
            </p>
            <p>
                <input type="submit" value="Submit" />
                <input type="reset" value="Reset" />
            </p>
        </fieldset>
    </form>
    <script>
        function sub() {
            // Function logic here
        }
    </script>
</body>
</html>





//employee registration form
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Employee Reg Form</title>
</head>
<body>
    <h1>Employee Registration Form</h1>
    <form action="welcome.html" method="get" novalidate>
        <fieldset>
            <legend>Personal Information</legend>
            <p>
                <label for="emp_name">Full Name:</label><br />
                <input type="text" id="emp_name" name="emp_name" required pattern="[A-Za-z]{3,50}" autocomplete="off" />
            </p>
            <p>
                <label for="emp_email">Email:</label><br />
                <input type="email" id="emp_email" name="emp_email" pattern="[a-zA-Z]+\.{1}[0-9]{6}@marwadiuniversity\.ac\.in" />
            </p>
            <p>
                <label for="emp_password">Password:</label><br />
                <input type="password" id="emp_password" name="emp_password" pattern="(?=.*[A-Z])(?=.*[a-z])(?=.*\d).{8,}" />
            </p>
            <p>
                <label for="emp_number">Phone number:</label><br />
                <input type="tel" id="emp_number" name="emp_number" pattern="[0-9]{10}" />
            </p>
            <p>
                <label for="emp_age">Age:</label><br />
                <input type="number" id="emp_age" name="emp_age" />
            </p>
            <p>
                <label for="address">Address:</label><br />
                <textarea id="address" name="address" rows="4" cols="50"></textarea>
            </p>
            <p>
                <label>Gender:</label><br />
                <input type="radio" id="gender_male" name="emp_gender" value="Male" checked />
                <label for="gender_male">Male</label>
                <input type="radio" id="gender_female" name="emp_gender" value="Female" />
                <label for="gender_female">Female</label>
            </p>
            <p>
                <label>Interests:</label><br />
                <input type="checkbox" id="interest_cricket" name="interests[]" value="Cricket" checked />
                <label for="interest_cricket">Cricket</label>
                <input type="checkbox" id="interest_hockey" name="interests[]" value="Hockey" />
                <label for="interest_hockey">Hockey</label>
                <input type="checkbox" id="interest_nothing" name="interests[]" value="Nothing" />
                <label for="interest_nothing">Nothing</label>
            </p>
        </fieldset>
        <fieldset>
            <legend>Preferences & Extras</legend>
            <p>
                <label for="emp_file">Upload Employee Photo:</label><br />
                <input type="file" id="emp_file" name="emp_file" multiple />
            </p>
            <p>
                <label for="fav_color">Badge Color:</label><br />
                <input type="color" id="fav_color" name="fav_color" />
            </p>
            <p>
                <label for="search_project">Search for Project:</label><br />
                <input type="search" id="search_project" name="search_project" />
            </p>
            <p>
                <label for="skill_range">Skill Level Range:</label><br />
                <input type="range" id="skill_range" name="skill_range" />
            </p>
            <p>
                <label for="emp_website">Portfolio Website:</label><br />
                <input type="url" id="emp_website" name="emp_website" pattern="https?://.+" />
            </p>
            <p>
                <label for="emp_dept">Department:</label><br />
                <select id="emp_dept" name="emp_dept[]" size="5" multiple>
                    <optgroup label="engg">
                        <option value="CE">CE</option>
                        <option value="EE" selected>EE</option>
                        <option value="ME">ME</option>
                        <option value="CIV">CIV</option>
                    </optgroup>
                    <optgroup label="Management">
                        <option value="BBA">BBA</option>
                        <option value="MBA">MBA</option>
                    </optgroup>
                </select>
            </p>
            <p>
                <label for="emp_country">Work Location Country: </label><br />
                <input list="countries" id="emp_country" name="emp_country" />
                <datalist id="countries">
                    <option value="USA">USA</option>
                    <option value="UK">UK</option>
                    <option value="India">India</option>
                    <option value="Japan">Japan</option>
                </datalist>
            </p>
            <p>
                <input type="checkbox" id="emp_agree" name="emp_agree" value="I agree" checked />
                <label for="emp_agree">Agree to Policy</label>
            </p>
        </fieldset>
        <fieldset>
            <legend>Date & Time Info</legend>
            <p>
                <label for="emp_date">Select Date of Joining:</label><br />
                <input type="date" id="emp_date" name="emp_date" />
            </p>
            <p>
                <label for="emp_time">Select Shift Time:</label><br />
                <input type="time" id="emp_time" name="emp_time" />
            </p>
            <p>
                <label for="emp_month">Select Joining Month:</label><br />
                <input type="month" id="emp_month" name="emp_month" />
            </p>
            <p>
                <label for="emp_week">Select Work Week:</label><br />
                <input type="week" id="emp_week" name="emp_week" />
            </p>
            <p>
                <label for="emp_datetime">Select Schedule Date and Time:</label><br />
                <input type="datetime-local" id="emp_datetime" name="emp_datetime" />
            </p>
        </fieldset>
        <fieldset>
            <legend>Form Controls</legend>
            <p>
                <button type="button" onclick="sub()">Click Me</button>
                <input type="image" src="" alt="Register Now" height="50" width="50" />
            </p>
            <p>
                <input type="submit" value="Submit" />
                <input type="reset" value="Reset" />
            </p>
        </fieldset>
    </form>
    <script>
        function sub() {
            // Function logic here
        }
    </script>
</body>
</html>
