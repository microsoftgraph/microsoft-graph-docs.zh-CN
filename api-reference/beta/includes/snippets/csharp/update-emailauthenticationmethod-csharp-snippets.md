---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 342951c1a86e8d8aa6fd25b2484328df07e36dbd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521311"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailAuthenticationMethod = new EmailAuthenticationMethod
{
    EmailAddress = "kim@contoso.com"
};

await graphClient.Users["kim@contoso.com"].Authentication.EmailMethods["3ddfcfc8-9383-446f-83cc-3ab9be4be18f"]
    .Request()
    .PutAsync(emailAuthenticationMethod);

```