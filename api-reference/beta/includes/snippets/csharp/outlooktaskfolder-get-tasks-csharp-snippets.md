---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef0cf8c6ea390ff3b646a948b151a9fbdc4cd759
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Outlook.TaskFolders["{outlookTaskFolder-id}"].Tasks
    .Request()
    .GetAsync();

```