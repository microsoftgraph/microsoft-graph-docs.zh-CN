---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: affce872657833f49486a55fd3aefaf1198708e3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806652"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucketTaskBoardTaskFormat = await graphClient.Planner.Tasks["{plannerTask-id}"].BucketTaskBoardFormat
    .Request()
    .GetAsync();

```