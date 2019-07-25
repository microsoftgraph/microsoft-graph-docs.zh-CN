---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c0ad2aa2970903af0f24f6e8eed3f7249d441c6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885569"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
user.accountEnabled = true;
user.displayName = "displayName-value";
user.mailNickname = "mailNickname-value";
user.userPrincipalName = "upn-value@tenant-value.onmicrosoft.com";
PasswordProfile passwordProfile = new PasswordProfile();
passwordProfile.forceChangePasswordNextSignIn = true;
passwordProfile.password = "password-value";
user.passwordProfile = passwordProfile;

graphClient.users()
    .buildRequest()
    .post(user);

```