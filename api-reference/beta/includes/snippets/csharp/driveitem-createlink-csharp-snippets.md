---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69ac55df9394b3e2edce01ad26959b71448cccdf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137747"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var scope = "anonymous";

var password = "String";

var recipients = new List<DriveRecipient>()
{
    new DriveRecipient
    {
    }
};

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,scope,null,password,null,recipients,null)
    .Request()
    .PostAsync();

```