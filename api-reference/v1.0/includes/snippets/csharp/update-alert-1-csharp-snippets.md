---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4767aa6997642c51010302631c0009b369582897
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945488"
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

await graphClient.Security.Alerts["{alert-id}"]
    .Request()
    .UpdateAsync(alert);

```