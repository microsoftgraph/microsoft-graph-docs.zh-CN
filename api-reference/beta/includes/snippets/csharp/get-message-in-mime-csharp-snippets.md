---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8cc559a7936802dbce880fd9705b162837d8861
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784151"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Messages["{message-id}"].Content
    .Request()
    .GetAsync();

```