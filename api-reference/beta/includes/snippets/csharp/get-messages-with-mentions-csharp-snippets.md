---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 326e62b864d399c768a608bfab6a7be792dedb6e69f671a385381a949b487126
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Filter("MentionsPreview/IsMentioned eq true")
    .Select("subject,sender,receivedDateTime,mentionsPreview")
    .GetAsync();

```