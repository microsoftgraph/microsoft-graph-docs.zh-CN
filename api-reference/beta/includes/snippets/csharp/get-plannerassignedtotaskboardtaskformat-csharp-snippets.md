---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92104ca8b36db6953d3a16ae094d43c894067e9f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerAssignedToTaskBoardTaskFormat = await graphClient.Planner.Tasks["01gzSlKkIUSUl6DF_EilrmQAKDhh"].AssignedToTaskBoardFormat
    .Request()
    .GetAsync();

```