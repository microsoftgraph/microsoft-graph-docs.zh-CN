---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c05f1f9f46833dd458e8c48fe5998cf69accd98
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].TokenIssuancePolicies["{tokenIssuancePolicy-id}"].Reference
    .Request()
    .DeleteAsync();

```