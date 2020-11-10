---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c0ad2aa2970903af0f24f6e8eed3f7249d441c6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977030"
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