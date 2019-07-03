---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 42a576ce62d79952db6ed54fcdee80334a9a2ec7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519678"
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