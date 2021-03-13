---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 548b6efadb81a84063104c0fed6b97ea4fb91766
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809645"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].TokenLifetimePolicies["{tokenLifetimePolicy-id}"].Reference
    .Request()
    .DeleteAsync();

```