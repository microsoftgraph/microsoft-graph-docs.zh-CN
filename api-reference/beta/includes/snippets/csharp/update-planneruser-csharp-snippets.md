---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b59c00c06df61008afbe2db159a12b7e64b9e37
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573230"
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
    .Header("Prefer","return=representation")
    .Header("If-Match","W/\"JzEtVXNlckRldGFpbHMgQEBAQEBAQEBAQEBAQEBIWCc=\"")
    .UpdateAsync(plannerUser);

```