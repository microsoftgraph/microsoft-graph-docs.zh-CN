---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55db84cb428e6ed0bd845f5738eeb2849ace4448
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683767"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Filter("MentionsPreview/IsMentioned eq true,")
    .Select("subject,sender,receivedDateTime,mentionsPreview")
    .GetAsync();

```