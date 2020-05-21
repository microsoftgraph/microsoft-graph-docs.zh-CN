---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7a275f0452aabc9b8398a82110d4094eca27189
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334416"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordCredential = new PasswordCredential
{
    DisplayName = "Password friendly name"
};

await graphClient.ServicePrincipals["{id}"]
    .AddPassword(passwordCredential)
    .Request()
    .PostAsync();

```