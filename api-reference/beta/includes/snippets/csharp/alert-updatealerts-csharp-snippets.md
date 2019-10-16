---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd5839134972f96b956599bdb1f8de32e75a3ef4
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544184"
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