---
title: 'Rental Application'
heading: Bakers Landing Rental Application
sub_heading:
sub_sub_heading:
page_url: faq
readmoretext: Have any questions? See our FAQ Page
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
        <input type="text" name="checkindate" value="{{ old:checkindate }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Check out Date</label>
        <input type="text" name="checkoutdate" value="{{ old:checkoutdate }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Name</label>
        <input type="text" name="name" value="{{ old:name }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Phone Number</label>
        <input type="text" name="phonenumber" value="{{ old:phonenumber }}" class="form-control" />
    </div>

    <div class="hidden form-group">
        <label>Username</label>
        <input type="text" name="username" />
    </div>

    <div class="form-group">
        <label>Email</label>
        <input type="email" name="email" value="{{ old:email }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Secondary Phone Number</label>
        <input type="text" name="secondaryphonenumber" value="{{ old:secondaryphonenumber }}" class="form-control" />
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
        <label>Number of years at address</label>
        <input type="text" name="numberyearsataddress" value="{{ old:numberyearsataddress }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Own/Rent</label>
        <select name="ownrent">
            <option value="">Please Select</option>
            <option value="Own">Own</option>
            <option value="Rent">Rent</option>
        </select>
    </div>

    <div class="form-group">
        <label>Business Phone</label>
        <input type="text" name="businessphone" value="{{ old:businessphone }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Extension</label>
        <input type="text" name="ext" value="{{ old:ext }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Employers Name</label>
        <input type="text" name="employersname" value="{{ old:employersname }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Employers Address</label>
        <input type="text" name="employersaddress" value="{{ old:employersaddress }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Job Title</label>
        <input type="text" name="jobtitle" value="{{ old:jobtitle }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Length of time employed at current job</label>
        <input type="text" name="lengthemployed" value="{{ old:lengthemployed }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Drivers License Number</label>
        <input type="text" name="driverslicensenumber" value="{{ old:driverslicensenumber }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>License Plate Number</label>
        <input type="text" name="licenseplatenumber" value="{{ old:licenseplatenumber }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Home/Renter Insurance Provider</label>
        <input type="text" name="homerenterinsurance" value="{{ old:homerenterinsurance }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Policy Number</label>
        <input type="text" name="policynumber" value="{{ old:policynumber }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Names, Addresses and Phone Numbers of ALL Adults and Children occupying Baker's Landing (including the ages of all children.)</label>
        <textarea name="alloccupants" class="form-control">{{ old:alloccupants }}</textarea>
    </div>

    <div class="form-group">
        <label>Are you bringing a Dog? A maximum of 2 dogs are allowed. Please provide details of age, breed ,size, temperament and training.</label>
        <textarea name="doginfo" class="form-control">{{ old:doginfo }}</textarea>
    </div>

    <div class="form-group">
        <label>Are you bringing any day or overnight Guests? Please provide their names and dates of their visit.</label>
        <textarea name="dayovernightguests" class="form-control">{{ old:dayovernightguests }}</textarea>
    </div>

    <div class="form-group">
        <label>Please use the area below to add any additional Details, Questions or Comments you may have.</label>
        <textarea name="comment" class="form-control">{{ old:comment }}</textarea>
    </div>

    <button class="btn btn-primary">Submit</button>

{{ /form:create }}
</article>
</article>
</section>
<section class="regular">
<article class="content rounded p-3 bright-blue-bg">
 <p class="white-text">You may fill in the Application Form above and click on <strong>Submit</strong> to submit the form via email.</p>

 <p class="white-text">Otherwise, if you would prefer to print or download a copy of Baker’s Landing Application Form click here. The Application Form will open in a new window. You will have different choices depending on your browser. Save, Print, Fill out form, email, download, etc… This Application Form is fill-able in adobe acrobat. After completing the Application Form you may email it back to us.</p>
</article>
</section>
