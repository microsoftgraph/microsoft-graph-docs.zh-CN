---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbca0e27dfdc313a819170d09af76384cb036b8e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212820"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var requestIds = new List<String>()
{
    "f01c6af6-6683-4a37-a945-0a925501eede",
    "42bf60ac-d0cb-4206-aa5c-101884298f55",
    "f09c8f14-8d8e-42cf-8a7e-732b0594e79b"
};

await graphClient.AuditLogs.SignIns
    .ConfirmCompromised(requestIds)
    .Request()
    .PostAsync();

```