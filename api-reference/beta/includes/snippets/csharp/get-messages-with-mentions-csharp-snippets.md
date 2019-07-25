---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 42a576ce62d79952db6ed54fcdee80334a9a2ec7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724059"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Filter("MentionsPreview/IsMentioned eq true,")
    .Select( e => new {
             e.Subject,
             e.Sender,
             e.ReceivedDateTime,
             e.MentionsPreview 
             })
    .GetAsync();

```