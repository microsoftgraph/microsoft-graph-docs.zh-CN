---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8c00e66b2e48a48daab61f11c8fd7da02657704d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<Alert>()
{
    new Alert
    {
        AssignedTo = "String",
        ClosedDateTime = "String (timestamp)",
        Comments = new List<String>()
        {
            "String"
        },
        Feedback = new AlertFeedback
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.type","microsoft.graph.alertFeedback"}
            }
        },
        Id = "String (identifier)",
        Status = new AlertStatus
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.type","microsoft.graph.alertStatus"}
            }
        },
        Tags = new List<String>()
        {
            "String"
        },
        VendorInformation = new SecurityVendorInformation
        {
            Provider = "String",
            Vendor = "String"
        }
    }
};

await graphClient.Security.Alerts
    .UpdateAlerts(value)
    .Request()
    .PostAsync();

```