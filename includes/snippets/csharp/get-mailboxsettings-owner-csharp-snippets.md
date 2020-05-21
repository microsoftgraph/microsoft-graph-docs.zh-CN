---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1471757657a4cb5a9d10b1dbe3015ca36c7fb50
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774797"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users["AlexW@contoso.OnMicrosoft.com"]
    .Request()
    .Select( e => new {
             e.MailboxSettings 
             })
    .GetAsync();

var mailboxSettings = users.MailboxSettings;

```