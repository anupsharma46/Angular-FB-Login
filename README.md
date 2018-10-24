# Angular-FB-Login

**1. Create a facebook application**

    Goto developer.facebook.com
    Login with your faceboob credential.
    Create New App, it will give you an Application ID for your new App.
    
**2. Create Angular Application using Angular CLI**   
    
**3. Install angular-6-social-login and setting up Facebook in your app**  
  - npm install --save angular-6-social-login 
  - Import SocialLoginModule, AuthServiceConfig, FacebookLoginProvider from angular-6-social-login in your app.module.ts
  - Add SocialLoginModule in imports array of @Ngmodule decorator in app.module.ts
  - Add below object in providers array in app.module.ts
    
        {
          provide: AuthServiceConfig,
          useFactory: getAuthServiceConfigs
        }
        
  - Include below code in app.module.ts and put your application ID in FacebookLoginProvider
             
              export function getAuthServiceConfigs() {

               let config = new AuthServiceConfig(
                  [
                    {
                      id: FacebookLoginProvider.PROVIDER_ID,
                      provider: new FacebookLoginProvider("Your Application ID")
                    }
                  ]);
                   return config;
              }
              
   - 
  **4. Create the components **
  
  **5. Compile and Run**
      ng serve --open
  
  
