---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c0cb3de21521deca2802ccd7e0b859fff8c9966
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080254"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Chats["{chat-id}"]
    .Request()
    .Expand("members")
    .GetAsync();

```