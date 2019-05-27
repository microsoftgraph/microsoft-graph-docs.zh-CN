---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c575ccd60a5c548dee2cfca68570c74c86c4ae06
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457339"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var me = await graphClient.Me
    .Request()
    .Select( e => new {
             e.MailboxSettings 
             })
    .GetAsync();

var mailboxSettings = me.MailboxSettings;

```