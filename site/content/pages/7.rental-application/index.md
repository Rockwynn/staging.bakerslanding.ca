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
        <input type="date" name="Check-In-Date" value="{{ old:Check-In-Date }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Check out Date</label>
        <input type="date" name="Check-Out-Date" value="{{ old:Check-Out-Date }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Name</label>
        <input type="text" name="Name" value="{{ old:Name }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Email</label>
        <input type="email" name="Email" value="{{ old:Email }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Home Phone Number</label>
        <input type="text" name="Home-Phone-Number" value="{{ old:Home-Phone-Number }}" class="form-control" />
    </div>

    <div class="hidden form-group">
        <label>Lastname</label>
        <input type="text" name="Lastname" />
    </div>

    <div class="form-group">
        <label>Cell Phone Number</label>
        <input type="text" name="Cell-Phone-Number" value="{{ old:Cell-Phone-Number }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Address</label>
        <input type="text" name="Address" value="{{ old:Address }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>City</label>
        <input type="text" name="City" value="{{ old:City }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Province/State</label>
        <input type="text" name="Province-State" value="{{ old:Province-State }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Postal Code/Zip Code</label>
        <input type="text" name="PostalCode-ZipCode" value="{{ old:PostalCode-ZipCode }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Number of years at present address</label>
        <input type="text" name="Number-of-Years-at-Address" value="{{ old:Number-of-Years-at-Address }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Do you Own or Rent your home</label>
        <select name="Owner-Renter" value="{{ old:Owner-Renter }}">
            <option value="">Please Select</option>
            <option value="Own">Own</option>
            <option value="Rent">Rent</option>
        </select>
    </div>

    <div class="form-group">
        <label>Employer's Name and Address:</label>
        <input type="text" name="Employer" value="{{ old:Employer }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Job Title:</label>
        <input type="text" name="Job-Title" value="{{ old:Job-Title }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Length of Employment at Current Job:</label>
        <input type="text" name="Length-of-Employment" value="{{ old:Length-of-Employment }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Driver's License Province/State and Number:</label>
        <input type="text" name="rivers-License" value="{{ old:Drivers-License }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Vehicle License Plate - Province/State and Number:</label>
        <input type="text" name="License-Plate" value="{{ old:License-Plate }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Home/Renter Insurance Provider:</label>
        <input type="text" name="Insurance-Provider" value="{{ old:Insurance-Provider }}" class="form-control" />
    </div>

    <div class="form-group">
        <label>Policy Number:</label>
        <input type="text" name="Policy-Number" value="{{ old:Policy-Number }}" class="form-control" />
    </div>










    <div class="form-group">
        <label>Number of Adults</label>
        <select name="Number-of-Adults" value="{{ old:Number-of-Adults }}">
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
        <select name="Number-of-Children" value="{{ old:Number-of-Children }}">
            <option value="">Please Select</option>
            <option value="1">1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
        </select>
    </div>

    <div class="form-group">
        <label>Names, Addresses and Phone Numbers of ALL Adults and Children occupying Baker’s Landing, including the ages of all children.</label>
        <textarea name="Occupant-Info" class="form-control">{{ old:Occupant-Info }}</textarea>
    </div>

    <div class="form-group">
        <label>Are you bringing a dog?</label>
        <select name="Bringing-Dog" value="{{ old:Bringing-Dog }}">
            <option value="">Please Select</option>
            <option value="Yes">Yes</option>
            <option value="No">No</option>
        </select>
    </div>

    <div class="form-group">
        <label>Please provide details of age, breed, size, temperament and training. Please note Baker's Landing has a strict "maximum 2 dog" policy, and cats are not allowed.</label>
        <textarea name="Dog-Info" class="form-control">{{ old:Dog-Info }}</textarea>
    </div>

    <div class="form-group">
        <label>Are you bringing any additional day or overnight guests?</label>
        <select name="Bringing-Guests" value="{{ old:Bringing-Guests }}">
            <option value="">Please Select</option>
            <option value="Yes">Yes</option>
            <option value="No">No</option>
        </select>
    </div>

    <div class="form-group">
        <label>If yes, please provide their names and dates of their visit.</label>
        <textarea name="Guest-Info" class="form-control">{{ old:Guest-Info }}</textarea>
    </div>

    <div class="form-group">
        <label>Do you plan on bringing a boat? If so we have plenty of parking space.</label>
        <select name="Bringing-Boat" value="{{ old:Bringing-Boat }}">
            <option value="">Please Select</option>
            <option value="Yes">Yes</option>
            <option value="No">No</option>
        </select>
    </div>

    <div><label class="blue-text">**Please note Baker's Landing holds a maximum of 8 persons, including babies and guests.**</label></div>

    <div class="form-group">
        <label>Please use the area below to add any additional details, special interests, questions or comments you may have.</label>
        <textarea name="Comment" class="form-control">{{ old:Comment }}</textarea>
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
