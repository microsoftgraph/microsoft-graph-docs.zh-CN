---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c9db24ae80cdcfffee6f215805fc22c67eaf6804
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479984"
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