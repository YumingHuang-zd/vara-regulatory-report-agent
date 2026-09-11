Please set the Entra ID Department field to exactly CRA for all active AI Team members.
Do not use security groups or app roles. Once updated, users with Logto SSO will receive CRA access automatically; users without Department=CRA will lose access.
Please confirm the number of users updated and any exceptions.



In Entra App Registration:
      - Remove the Microsoft Graph delegated permission User.Read.All.
      - Add the Microsoft Graph delegated permission User.Read (e1fe6dd8-ba31-4d61-89e7-88639da4683d).
      - Keep the Microsoft Graph application permission User.Read.All (df021288-bdef-4463-88db-98f22de89214) for
        the existing Department/CRA sync job.
 
      - Remove the existing tenant-wide delegated User.Read.All consent grant, then grant tenant-wide admin
        consent for User.Read.
