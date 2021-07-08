---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd16c887c615c15b7d639b36e64047510de2566d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316512"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
PasswordProfile passwordProfile = new PasswordProfile();
passwordProfile.forceChangePasswordNextSignIn = false;
passwordProfile.password = "xWwvJ]6NMw+bWH-d";
user.passwordProfile = passwordProfile;

graphClient.users("{id}")
    .buildRequest()
    .patch(user);

```