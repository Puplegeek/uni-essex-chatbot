---
key: expertise/case-studies/blackman-&-white
page_url: https://www.essex.ac.uk/business/expertise/case-studies/blackman-&-white
scraped_at: 2025-05-21 00:59:51
---

# Server Error in '/' Application. ---

## *Runtime Error*


 **Description:** An application error occurred on the server. The current custom error settings for this application prevent the details of the application error from being viewed remotely (for security reasons). It could, however, be viewed by browsers running on the local server machine.
  
  
**Details:** To enable the details of this specific error message to be viewable on remote machines, please create a <customErrors> tag within a "web.config" configuration file located in the root directory of the current web application. This <customErrors> tag should then have its "mode" attribute set to "Off".  
  

|  |
| --- |
| ````  <!-- Web.Config Configuration File -->  <configuration>     <system.web>         <customErrors mode="Off"/>     </system.web> </configuration> ```` |

  
**Notes:** The current error page you are seeing can be replaced by a custom error page by modifying the "defaultRedirect" attribute of the application's <customErrors> configuration tag to point to a custom error page URL.  
  

|  |
| --- |
| ````  <!-- Web.Config Configuration File -->  <configuration>     <system.web>         <customErrors mode="RemoteOnly" defaultRedirect="mycustompage.htm"/>     </system.web> </configuration> ```` |