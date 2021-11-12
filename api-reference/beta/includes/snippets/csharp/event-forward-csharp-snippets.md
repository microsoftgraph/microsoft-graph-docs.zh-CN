---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d52239fa69c5c287baf653ee97d54f7801d926465121eda9d35e18f5f360bc96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var toRecipients = new List<Recipient>()
{
    new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Address = "danas@contoso.onmicrosoft.com",
            Name = "Dana Swope"
        }
    }
};

var comment = "Dana, hope you can make this meeting.";

await graphClient.Me.Events["{event-id}"]
    .Forward(toRecipients,comment)
    .Request()
    .PostAsync();

```