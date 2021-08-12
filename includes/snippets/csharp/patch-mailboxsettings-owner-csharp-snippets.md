---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fada4de5a8a5b8918057789f647dbca94619b84df63a3535970c5ea090988c5e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237030"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailboxSettings = new MailboxSettings
{
    DelegateMeetingMessageDeliveryOptions = DelegateMeetingMessageDeliveryOptions.SendToDelegateAndPrincipal
};

var users = new User();
users.MailboxSettings = mailboxSettings;

await graphClient.Users["AlexW@contoso.OnMicrosoft.com"]
    .Request()
    .UpdateAsync(users);

```