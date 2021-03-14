---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ed346f3d9be9fa14d98c51ff67e3594d2df0734
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799685"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTaskDetails = new PlannerTaskDetails
{
    PreviewType = PlannerPreviewType.NoPreview,
    References = new PlannerExternalReferences
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"http%3A//developer%2Emicrosoft%2Ecom", "{\"@odata.type\":\"microsoft.graph.plannerExternalReference\",\"alias\":\"Documentation\",\"previewPriority\":\" !\",\"type\":\"Other\"}"},
            {"https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer", "{\"@odata.type\":\"microsoft.graph.plannerExternalReference\",\"previewPriority\":\"  !!\"}"},
            {"http%3A//www%2Ebing%2Ecom", "null"}
        }
    },
    Checklist = new PlannerChecklistItems
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"95e27074-6c4a-447a-aa24-9d718a0b86fa", "{\"@odata.type\":\"microsoft.graph.plannerChecklistItem\",\"title\":\"Update task details\",\"isChecked\":true}"},
            {"d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff", "{\"@odata.type\":\"microsoft.graph.plannerChecklistItem\",\"isChecked\":true}"},
            {"a93c93c5-10a6-4167-9551-8bafa09967a7", "null"}
        }
    }
};

await graphClient.Planner.Tasks["{plannerTask-id}"].Details
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerTaskDetails);

```