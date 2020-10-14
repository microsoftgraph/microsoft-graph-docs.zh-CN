---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ef8a0377dc14ab702ea3699734530192933527e
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457555"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newPassword = "newPassword-value";

await graphClient.Users["{id | userPrincipalName}"].Authentication.PasswordMethods["{id}"]
    .ResetPassword(newPassword,null)
    .Request()
    .PostAsync();

```