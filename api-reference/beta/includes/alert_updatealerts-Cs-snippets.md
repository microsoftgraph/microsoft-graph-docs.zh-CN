---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c9db24ae80cdcfffee6f215805fc22c67eaf6804
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451999"
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
        },
        Id = "String (identifier)",
        Status = new AlertStatus
        {
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