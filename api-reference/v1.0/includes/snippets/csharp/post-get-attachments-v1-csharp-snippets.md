---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31470f23a1c0d524edf8fa777d98ccb45ff41ea6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts["{post-id}"].Attachments
    .Request()
    .GetAsync();

```