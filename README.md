#Roles
CP: Content Provider
AAPP: Android App Publication Platform
AADP: Android App Distribution Platform


# Rules - The rules to publish your App.

CP1---\         /---(audit)----AADP1----Users
CP2---- AAPP----(audit)----AADP2----Users
CPn--/          \---(audit)----AADPn----Users

1. A CP creates a xml file when he registers a new app or updates the xml file when he updates the app;
    The xml file must match the versionN.xsd(version1.xsd currently) schema, and is push to the Apps project.
2. These github projects are named as AAPP, including Rules and Apps.
3. Each AADP, for example a Appstore, is monitoring the AAPP and audits the changed Apps;
    The AADP could decide which Apps are passed accoriding to itself's review conditons.
4. AADP will distribute the apps to users on its media positions.

#Notes 
AAPP is a public organization which assumes no responsibility for the security and the copyright of this informations, 
one or more github users are assumed as the owner of a xml file, the owner part in the xml file should be same with the github users,
but you can submit a pull request to the github to update the owner part of a xml file if your copyright is violated.    
