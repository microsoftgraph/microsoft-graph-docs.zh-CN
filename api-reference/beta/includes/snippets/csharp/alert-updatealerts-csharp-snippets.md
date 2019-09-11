---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5076a86f82b9d870fa2bd4b27d500f7376581838
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845935"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<Alert>()
{
    new Alert
    {
        AssignedTo = "String",
        ClosedDateTime = DateTimeOffset.Parse("String (timestamp)"),
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