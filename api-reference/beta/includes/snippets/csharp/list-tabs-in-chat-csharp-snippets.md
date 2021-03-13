---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5372f35c0356c4ab1a44c72326fedf60166b304
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775785"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Chats["{chat-id}"].Tabs
    .Request()
    .Expand("teamsApp")
    .GetAsync();

```