---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d3157ba272e4e2edbbe6ea20cb180e038f45b72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.EmailMethods["{emailAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```