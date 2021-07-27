---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16e414a7f3a31cb3e0f8f0da97760a3789e55a05
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580870"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodsPolicy = await graphClient.Policies.AuthenticationMethodsPolicy
    .Request()
    .GetAsync();

```