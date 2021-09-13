---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7538c12db6d08abd2889b085d3203cf244a1a64d72f6a4004cdc2fa3999c1b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218705"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = new PlannerBucket
{
    Name = "Development"
};

await graphClient.Planner.Buckets["{plannerBucket-id}"]
    .Request()
    .Header("Prefer","return=representation")
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerBucket);

```