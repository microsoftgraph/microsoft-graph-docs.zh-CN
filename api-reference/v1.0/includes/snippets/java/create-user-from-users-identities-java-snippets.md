---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d23654993f70abb26c475d262a225bc4183fc05
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081330"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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