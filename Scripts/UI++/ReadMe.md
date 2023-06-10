## UI++ template
### Template to automate and create interactive options for desktop support when doing image deployments. <br><br>
I created this template and integrated it with SCCM to allow easier image deployments for environments with different computer builds and regions.
Features include setting a computer name, choosing a region, OU, choosing a specific computer build. <br><br>
The login screen will verify the user running the deployment is authorized by an AD query that looks at group DeskstopImagingGroup. <br><br>
This template will allow passing variables to a task sequence when having multiple regions and OU structure tied to regions. <br><br>
The region variable can be used in a task sequence to set region specific settings such as time, keyboard options, etc. <br><br>
When setting the computer name an AD query will see if it's already in use. <br><br>

UI++ download and documentation<br>
https://uiplusplus.configmgrftw.com/
