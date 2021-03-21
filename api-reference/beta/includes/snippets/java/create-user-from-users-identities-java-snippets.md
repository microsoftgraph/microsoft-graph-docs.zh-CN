---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a705cf6cd369cd23bbdc4668f26adf9db1f4bb3b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981071"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
user.displayName = "John Smith";
LinkedList<ObjectIdentity> identitiesList = new LinkedList<ObjectIdentity>();
ObjectIdentity identities = new ObjectIdentity();
identities.signInType = "userName";
identities.issuer = "contoso.onmicrosoft.com";
identities.issuerAssignedId = "johnsmith";
identitiesList.add(identities);
ObjectIdentity identities1 = new ObjectIdentity();
identities1.signInType = "emailAddress";
identities1.issuer = "contoso.onmicrosoft.com";
identities1.issuerAssignedId = "jsmith@yahoo.com";
identitiesList.add(identities1);
ObjectIdentity identities2 = new ObjectIdentity();
identities2.signInType = "federated";
identities2.issuer = "facebook.com";
identities2.issuerAssignedId = "5eecb0cd";
identitiesList.add(identities2);
user.identities = identitiesList;
PasswordProfile passwordProfile = new PasswordProfile();
passwordProfile.password = "password-value";
passwordProfile.forceChangePasswordNextSignIn = false;
user.passwordProfile = passwordProfile;
user.passwordPolicies = "DisablePasswordExpiration";

graphClient.users()
    .buildRequest()
    .post(user);

```