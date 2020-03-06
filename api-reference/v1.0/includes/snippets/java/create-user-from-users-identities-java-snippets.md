---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 644578bcf826499afad236e9021daffed6536917
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558811"
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
user.passwordProfile = passwordProfile;
user.passwordPolicies = "DisablePasswordExpiration";

graphClient.users()
    .buildRequest()
    .post(user);

```