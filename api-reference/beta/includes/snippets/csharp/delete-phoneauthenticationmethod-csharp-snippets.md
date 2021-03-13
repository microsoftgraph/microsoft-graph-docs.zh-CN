---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8acb705b27ec0803e5c754f53ab13f402c390c28
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Authentication.PhoneMethods["{phoneAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```