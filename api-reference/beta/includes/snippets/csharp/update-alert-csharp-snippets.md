---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 956a08b8bdf852748cee328fd8264b90106d3244
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845934"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = new Alert
{
    AssignedTo = "String",
    ClosedDateTime = DateTimeOffset.Parse("String (timestamp)"),
    Comments = new List<String>()
    {
        "String"
    },
    Feedback = AlertFeedback.Unknown,
    Status = AlertStatus.Unknown,
    Tags = new List<String>()
    {
        "String"
    },
    VendorInformation = new SecurityVendorInformation
    {
        Provider = "String",
        Vendor = "String"
    }
};

await graphClient.Security.Alerts["{alert_id}"]
    .Request()
    .Header("Prefer","return=representation")
    .UpdateAsync(alert);

```