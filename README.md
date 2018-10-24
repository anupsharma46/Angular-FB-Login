# Angular-FB-Login

**1. Create a facebook application**

    Goto developer.facebook.com
    Login with your credential.
    Create New App, it will give you an Application ID for your new App.
    
**2. Create Angular Application using Angular CLI**   
    
**3. Install angular-6-social-login and setup Facebook in your app**  
  - npm install --save angular-6-social-login 
  - Import SocialLoginModule, AuthServiceConfig, FacebookLoginProvider from angular-6-social-login in your app.module.ts
  - Add SocialLoginModule in imports array of @Ngmodule decorator in app.module.ts
  - Add below object in providers array in app.module.ts
    
        {
          provide: AuthServiceConfig,
          useFactory: getAuthServiceConfigs
        }
        
  - Put your application ID in provider on line 21 in app.module.ts
  
  **4.**
  
  
