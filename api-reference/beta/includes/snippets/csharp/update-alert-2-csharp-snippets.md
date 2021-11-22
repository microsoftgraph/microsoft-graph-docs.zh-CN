---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09da7088d8e8a72d32ca21ea3b3cfd8ddcb0fb85469c910bb58f8d25df9a1f4d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215738"
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
    .Header("Prefer","return=representation")
    .UpdateAsync(alert);

```