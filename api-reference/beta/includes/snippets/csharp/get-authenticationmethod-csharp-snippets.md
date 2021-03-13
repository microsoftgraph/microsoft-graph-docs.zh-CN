---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f419cdf6e1f1f0e187ffec7be9ab5ad1e03beeef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803762"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethod = await graphClient.Me.Authentication.Methods["{authenticationMethod-id}"]
    .Request()
    .GetAsync();

```