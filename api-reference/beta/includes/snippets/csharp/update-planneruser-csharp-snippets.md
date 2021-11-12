---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 903b40bf1d03e568081427883cbec412b7c749156f7549eb8dec6a3ef316ddb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220618"
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