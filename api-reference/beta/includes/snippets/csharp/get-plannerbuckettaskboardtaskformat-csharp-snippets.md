---
description: 自动生成的文件。 不修改
ms.openlocfilehash: db4c13d8b3bd2fd94e34ce6dc45c486733b9167e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480120"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucketTaskBoardTaskFormat = await graphClient.Planner.Tasks["01gzSlKkIUSUl6DF_EilrmQAKDhh"].BucketTaskBoardFormat
    .Request()
    .GetAsync();

```