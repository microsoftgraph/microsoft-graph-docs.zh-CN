---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 551c2c772b747b54573326005f9b20c10ec5e37e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801179"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Me.Assignments["{educationAssignment-id}"].Rubric.Reference
    .Request()
    .DeleteAsync();

```