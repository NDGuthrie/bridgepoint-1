---

This work is licensed under the Creative Commons CC0 License

---

# xtUML.org Website Migration Project
### xtUML Project Analysis Note


1. Abstract
-----------
1.1 - The purpose of this project is to migrate the exisiting webiste www.xtuml.org from its current hosted location, 
which utilizes Amazon web services (AWS), to another location, specifically GoDaddy (www.godaddy.com).

2. Document References
----------------------

[1] [BridgePoint DEI #1](https://support.onefact.net/redmine/issues/611)  
[2] [GoDaddy.com] (https://support.godaddy.com/help/article/8997/migrating-your-site-to-managed-wordpress)

[3] [GoDaddy.com] (https://support.godaddy.com/help/article/6117/moving-your-wordpress-site-to-us-from-another-host)

[4] [WordPress.com] (http://en.support.wordpress.com/export/)


3. Background
-------------

3.1 - xtuml.org is hosted on a server owned and controled by OneFact.

3.2 - This server is an instance hosted on AWS.

3.3 - AWS costs something like $100+ per month.

3.4 - GoDaddy for onefact.net costs $1 per month.

3.5 - xtuml.org is a web site.  It does not need to run on a standalone server.

3.6 - xtuml.org should be hosted in a hosting environment like GoDaddy.


4. Requirements
---------------

4.1 - The new website shall support the forum.
4.2 - The new website shall contain the existing forum topics & replies.
4.3 - The new website shall support WP Courseware.
4.4 - The new website shall maintain the progress of users in the courses.
4.5 - Existing user registrations shall carry over to the new site.
4.6 - The website shall include anti-spam measures on the forum and user registration.
4.7 - Interruptions in xtuml.org availability must be kept low - Interruptions of more than an hour are not acceptable.
4.8 - The cost of maintaining the site must be reduced - xtuml.org must cost less than $50 per month and preferably 
be around $1 per month.
4.9 - Minimize "departures from standards" that make the site difficult to maintain.
4.10 - Use off-the-shelf themes and plugins whenever practical.
4.11 - xtuml.net and xtuml.com exist, and they shall temporarily serve as a staging area for the migration.
4.12 - xtuml.net and xtuml.com shall forward to the same new website when the migration is completed.


5. Analysis
-----------

5.1 - An attempt was made to use the tool provided by GoDaddy.com to migrate the existing xtUML.org WordPress site 
to a GoDaddy.com host. However, this attempt was unsuccessful.
5.2 - Initial research.  There is a function on the WordPress Dashboard called "Export".  According to [4], 
this function will download all content of the WordPress site to a local host. 
5.3.1 - Option 1. The data may be exported to a local host.  This data may be used as a file to "Import" on the new 
WordPress site hosted by GoDaddy.com by using the "Import" function on the WordPress Dashboard.
5.3.2 - Option 2.  Another option for migrating from the existing WordPress xtUML.org site to a site hosted by 
GoDaddy.com is to use the manual method as described in [3].  This method is more invovled because it involves 
working with the MySQL and PHPMyAdmin configurations.  Care must be taken here.
5.4 - Unknowns: Given the nature of WordPress and its use of plugins, it is not known if the plugins currently 
utilized by the xtUML.org WordPress site are specific to Amazon Web Services, or are non-premium 
(read: "freely available").  In response to the requirements in Section 4 above, the following statements should be 
verified.
5.4.1 - The proposed GoDaddy host supports the existing forum plugin.
5.4.2 - The proposed GoDaddy host supports the WP Courseware.
5.4.3 - The proposed GoDaddy host supports the migration of existing user registrations.
5.5 - It seems likely that these features are supported by GoDaddy.com since all WordPress websites are designed to be 
compatible, but it is unknown for certain at the time of this writing.

6. Work Required
----------------
6.1 - Proposed work: A simple and effective next step to migrate the existing xtUML.org website would be to use 
the existing xtUML.org WordPress site's Export feature from the Dashboard to create a backup of the existing 
xtUML.org website. 
6.2 - This backup file may be imported to the proposed GoDaddy.com host.  
6.3 - When these steps are completed, it would be a matter of seeing what works on the new site and what does not.  
6.4 - The existing site remains unchanged with no downtime.

7. Acceptance Test
------------------

7.1 - Check the new website to see if the forum is supported and functional.
7.2 - Check the new website to see if it contains the existing forum topics & replies.
7.3 - Check the new website to see if it supports WP Courseware.
7.4 - Check the new website to see if it maintains the progress of users in the courses.
7.5 - Check the new website to see if existing user registrations carry over to the new site.
7.6 - Check the new website to see if it includes anti-spam measures on the forum and user registration.
7.7 - Interruptions in xtuml.org availability will be kept low - the export feature of the WordPress site should not
interfere with the availability of xtuml.org.
7.8 - The cost of maintaining the site should be reduced to around $1 per month.
7.9 - Minimize "departures from standards" that make the site difficult to maintain.
7.10 - Use off-the-shelf themes and plugins whenever practical.
4.11 - xtuml.net and xtuml.com exist, and they may be checked to determine that they temporarily serve as a staging 
area for the migration.
4.12 - xtuml.net and xtuml.com may be checked to determine that they forward to the same new website when the 
migration is completed.


End
---

