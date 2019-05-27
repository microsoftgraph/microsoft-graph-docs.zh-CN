---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a80fb78f3efb9a70b6626b4ee1782494ad65c9a1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var EmailAddresses = new List<String>()
{
    "danas@contoso.onmicrosoft.com",
    "fannyd@contoso.onmicrosoft.com"
};

var MailTipsOptions = "automaticReplies, mailboxFullStatus";

await graphClient.Me
    .GetMailTips(emailAddresses,mailTipsOptions)
    .Request()
    .PostAsync();

```