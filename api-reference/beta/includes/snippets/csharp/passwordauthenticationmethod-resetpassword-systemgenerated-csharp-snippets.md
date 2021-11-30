---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44a46b9a68398636e2f9455617f95bc205f79b7abe1ec57f0639f0ab4ad1c923
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279113"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.PasswordMethods["{passwordAuthenticationMethod-id}"]
    .ResetPassword(null,null)
    .Request()
    .PostAsync();

```