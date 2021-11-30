---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 103d2626591cf9868fd30d51f6a15ace6b49d881e723cb88f593cca12066cb1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164338"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newPassword = "newPassword-value";

await graphClient.Users["{user-id}"].Authentication.PasswordMethods["{passwordAuthenticationMethod-id}"]
    .ResetPassword(newPassword,null)
    .Request()
    .PostAsync();

```