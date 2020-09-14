---
title: 'Rental Application'
heading: 'Bakers Landing Rental Application'
page_url: faq
readmoretext: 'Have any questions? See our FAQ Page'
fieldset: default
template: about
id: 41b0e0b7-0426-41ad-9c6e-8a7325fb5a95
---
<article class="content">
{{ form:create in="rental-application" }}

    {{ if errors }}
        <div class="alert alert-danger">
            {{ errors }}
                {{ value }}<br>
            {{ /errors }}
        </div>
    {{ /if }}

    {{ if success }}
        <div class="alert alert-success">
            Form was submitted successfully.
        </div>
    {{ /if }}

    <div class="form-group">
        <label>Check in Date - Saturday</label>
        <input type="date" name="checkindate" value="{{ old:checkindate }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Check out Date</label>
        <input type="date" name="checkoutdate" value="{{ old:checkoutdate }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Name</label>
        <input type="text" name="name" value="{{ old:name }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Email</label>
        <input type="email" name="email" value="{{ old:email }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Home Phone Number</label>
        <input type="text" name="homephonenumber" value="{{ old:homephonenumber }}" class="form-control" />
    </div>

    <div class="hidden form-group">
        <label>Username</label>
        <input type="text" name="username" />
    </div>

    <div class="form-group">
        <label>Cell Phone Number</label>
        <input type="text" name="cellphonenumber" value="{{ old:cellphonenumber }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Address</label>
        <input type="text" name="address" value="{{ old:address }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>City</label>
        <input type="text" name="city" value="{{ old:city }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Province/State</label>
        <input type="text" name="provincestate" value="{{ old:provincestate }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Postal Code/Zip Code</label>
        <input type="text" name="postalzipcode" value="{{ old:postalzipcode }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Number of years at present address</label>
        <input type="text" name="numberyearsataddress" value="{{ old:numberyearsataddress }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Do you Own or Rent your home</label>
        <select name="ownrent">
            <option value="">Please Select</option>
            <option value="Own">Own</option>
            <option value="Rent">Rent</option>
        </select>
    </div>





    <div class="form-group">
        <label>Employer's Name and Address:</label>
        <input type="text" name="employer" value="{{ old:employer }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Job Title:</label>
        <input type="text" name="jobtitle" value="{{ old:jobtitle }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Length of Employment at Current Job:</label>
        <input type="text" name="lengthofemployment" value="{{ old:lengthofemployment }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Driver's License Province/State and Number:</label>
        <input type="text" name="driverslicense" value="{{ old:driverslicense }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Vehicle License Plate - Province/State and Number:</label>
        <input type="text" name="licenseplate" value="{{ old:licenseplate }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Home/Renter Insurance Provider:</label>
        <input type="text" name="insuranceprovider" value="{{ old:insuranceprovider }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Policy Number:</label>
        <input type="text" name="policynumber" value="{{ old:policynumber }}" class="form-control" />
    </div>










    <div class="form-group">
        <label>Number of Adults</label>
        <select name="numberadults">
            <option value="">Please Select</option>
            <option value="1">1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
        </select>
    </div>

    <div class="form-group">
        <label>Number of Children</label>
        <select name="numberchildren">
            <option value="">Please Select</option>
            <option value="1">1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
        </select>
    </div>

    <div class="form-group">
        <label>Are you bringing a dog?</label>
        <select name="bringingdog">
            <option value="">Please Select</option>
            <option value="Yes">Yes</option>
            <option value="No">No</option>
        </select>
    </div>

    <div class="form-group">
        <label>Please provide details of age, breed, size, temperament and training. Please note Baker's Landing has a strict "maximum 2 dog" policy, and cats are not allowed.</label>
        <textarea name="doginfo" class="form-control">{{ old:doginfo }}</textarea>
    </div>

    <div class="form-group">
        <label>Are you bringing any additional day or overnight guests?</label>
        <select name="bringingguests">
            <option value="">Please Select</option>
            <option value="Yes">Yes</option>
            <option value="No">No</option>
        </select>
    </div>

    <div class="form-group">
        <label>If yes, please provide their names and dates of their visit.</label>
        <textarea name="guestinfo" class="form-control">{{ old:guestinfo }}</textarea>
    </div>

    <div class="form-group">
        <label>Do you plan on bringing a boat? If so we have plenty of parking space.</label>
        <select name="bringingboat">
            <option value="">Please Select</option>
            <option value="Yes">Yes</option>
            <option value="No">No</option>
        </select>
    </div>

    <div><label class="blue-text">**Please note Baker's Landing holds a maximum of 8 persons, including babies and guests.**</label></div>

    <div class="form-group">
        <label>Please use the area below to add any additional details, special interests, questions or comments you may have.</label>
        <textarea name="comment" class="form-control">{{ old:comment }}</textarea>
    </div>

    <div><label>Privacy Policy: The owners of Baker’s Landing will keep all information collected private. The information is being collected for rental screening purposes.</label></div>

    <button class="btn btn-primary">Submit</button>

{{ /form:create }}
</article>
</article>
</section>
<section class="regular">
<article class="content rounded p-3 bright-blue-bg">
 <p class="white-text">You may fill in the Application Form above and click on submit, to submit via email. Otherwise, if you would prefer to print or download a copy of the Baker's Landing Application Form <a href="/Bakers-Landing-Application-Form.pdf"><strong>click here</strong></a>. The Application Form will open in a new window. You will have different choices depending on your browser. Save, Print, Fill out form, email, download, etc… This Application Form is fill-able in adobe acrobat. After completing the Application Form you may email it back to us.</p>
</article>
</section>
