# Acoustic Preference Center

Code base for hosting a preference center in Acoustic Campaign that allows for Sign Ups, Snoozing and Unsubscribing.

This will submit to a database in Acoustic Campaign. Bootstrap (5.1.3) framework was used for HTML and jQuery was used for javascript library because those are what I am familiar with. This code is intended to be pasted in source code for a Landing Page's new created Page which allows for Acoustic to host the forms. 

In addition to just getting data into Acoustic Campaign here are the other features

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

I've created <a href="https://marketingsoultions.guru/wp-live/creating-a-single-preference-center-for-sign-ups-unsubscribing-and-snoozing-for-acoustic-campaign/" target="_blank">a blog post here</a> that is used as a walk through for setting this up in your own Acoustic instance.