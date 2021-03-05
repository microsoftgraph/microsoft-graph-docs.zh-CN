---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26a47a1554789840c9f461e68882c5a72533b39a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474031"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerUser = new PlannerUser
{
    FavoritePlanReferences = new PlannerFavoritePlanReferenceCollection
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"jd8S5gOaFk2S8aWCIAJz42QAAxtD", "{\"@odata.type\":\"#microsoft.graph.plannerFavoritePlanReference\",\"orderHint\":\" !\",\"planTitle\":\"Next Release Discussion\"}"},
            {"7oTB5aMIAE2rVo-1N-L7RmQAGX2q", "null"}
        }
    },
    RecentPlanReferences = new PlannerRecentPlanReferenceCollection
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"jd8S5gOaFk2S8aWCIAJz42QAAxtD", "{\"@odata.type\":\"#microsoft.graph.plannerRecentPlanReference\",\"lastAccessedDateTime\":\"2018-01-02T22:49:46.155Z\",\"planTitle\":\"Next Release Discussion\"}"}
        }
    }
};

await graphClient.Me.Planner
    .Request()
    .Header("If-Match","W/\"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc=\"")
    .UpdateAsync(plannerUser);

```