# Acoustic Preference Center
<h3>Overview</h3>
This is the code base for hosting a preference center in Acoustic Campaign that allows for Sign Ups, Snoozing and Unsubscribing.

This will submit to a database in Acoustic Campaign. Bootstrap (5.1.3) framework was used for HTML and jQuery was used for javascript library because those are what I am familiar with. This code is intended to be pasted in source code for a Landing Page's new created Page which allows for Acoustic to host the forms.

I've created <a href="https://marketingsoultions.guru/wp-live/creating-a-single-preference-center-for-sign-ups-unsubscribing-and-snoozing-for-acoustic-campaign/" target="_blank">a blog post here</a> that is used as a walk through for setting this up in your own Acoustic instance.

<hr>

<h3>Goals</h3>
<ul>
	<li>Submit entries to Acoustic Campaign's Database</li>
	<li>Independent confirmation messages for successful sign up, snoozing and unsubscribing</li>
	<li>Clear call to action for someone to fully unsubscribe</li>
	<li>Proper validation of required fields, even dynamic fields. IE if sms is selected require phone</li>
</ul>

<hr>

<h3>Feature List</h3>
<ul>
	<li>Pre-Populates Entire form for existing subscribes via URL parameters</li>
	<li>If zip is filled out City and State will be populated via Google API</li>
	<li>If SMS is selected the Phone becomes a required field</li>
	<li>Custom messages for required fields</li>
	<li>If a subscriber is opt’d in to a subscription the toggle will display their opt’d in fields for that property</li>
	<li>Snooze and Unsubscribe row only shows if email value is present</li>
	<li>Unsubscribe Popover will appear if unsubscribe parameter has any value</li>
</ul>
<hr>
<h3>Developer Requirements</h3>
In order for this to work properly the following will need to be done:
<ul>
	<li>Create landing page in Acoustic</li>
	<li>Associate landing page to Contact Source with columns you'd like to display</li>
	<li>Create Sign Up form with a snooze option and other desired fields</li>
	<li>Create Unsubscribe form with desired fields</li>
	<li>Update Google Geocode API with your key</li>
	<li>Uploading source code to</li>
	<ul>
		<li>Page's Source Code</li>
		<li>Confirmation page for Sign Up</li>
		<li>Confirmation page for Unsubscribe</li>
	</ul>
	<li>Update Google Captcha Code</li>
</ul>


<hr>
<h3>Dependencies</h3>
<table>
	<thead>
		<tr>
			<th align="center">Library</th>
			<th align="left">Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td align="center">Bootstrap v5.1</td>
			<td align="left">Frontend framework.</td>
		</tr>
		<tr>
			<td align="center">Popper Javascript</td>
			<td align="left">Pop up calling attention to Unsubscribe button when certain variables are passed</td>
		</tr>
		<tr>
			<td align="center">Fontawesome</td>
			<td align="left">Used for icons</td>
		</tr>
		<tr>
			<td align="center">jQuery v1.12</td>
			<td align="left">Javascript library used for validation, populating fields via api, etc.</td>
		</tr>
		<tr>
			<td align="center">jQuery Validate v1.19</td>
			<td align="left">Library used for validation fields and creating rules for specific validation needs</td>
		</tr>
	</tbody>
</table>