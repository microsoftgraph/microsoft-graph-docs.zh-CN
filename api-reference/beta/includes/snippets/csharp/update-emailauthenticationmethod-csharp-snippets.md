---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae9ac3d90de386edddd0c962ab85f5a18027b599860f85d03127cacefcfb79db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274006"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailAuthenticationMethod = new EmailAuthenticationMethod
{
    EmailAddress = "kim@contoso.com"
};

await graphClient.Users["{user-id}"].Authentication.EmailMethods["{emailAuthenticationMethod-id}"]
    .Request()
    .PutAsync(emailAuthenticationMethod);

```