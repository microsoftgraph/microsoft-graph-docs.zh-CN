---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21738a1db7a83f8be6a6ffa753a076a35c4b33b7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806234"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = await graphClient.Me.Outlook.Tasks["{outlookTask-id}"]
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .GetAsync();

```