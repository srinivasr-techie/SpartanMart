# SpartanMart
SAP Commerce Cloud 2211 spartacus storefront

# Below are the sample sym links created for the repo to SAP Commerce suite
mklink /J "D:\Hybris\SpartanMart\2211\hybris\bin\custom" "D:\Hybris\SpartanMart\Repo\core-customize\hybris\bin\custom"
mklink /J "D:\Hybris\SpartanMart\2211\installer\recipes\cx_spartan_occ" "D:\Hybris\SpartanMart\Repo\core-customize\installer\recipes\cx_spartan_occ"
mklink "D:\Hybris\SpartanMart\2211\installer\customconfig\custom.properties" "D:\Hybris\SpartanMart\Repo\core-customize\hybris\bin\custom\spartacussampledata\resources\installer\customconfig\custom.properties"

# OCC Credentials
INSERT_UPDATE OAuthClientDetails;clientId[unique=true]    ;resourceIds       ;scope        ;authorizedGrantTypes                                            ;authorities             ;clientSecret    ;registeredRedirectUri
                                ;client-side              ;hybris            ;basic        ;implicit,client_credentials                                     ;ROLE_CLIENT             ;secret          ;http://localhost:9001/authorizationserver/oauth2_implicit_callback;
                                ;mobile_android           ;hybris            ;basic        ;authorization_code,refresh_token,password,client_credentials    ;ROLE_CLIENT             ;secret          ;http://localhost:9001/authorizationserver/oauth2_callback;