---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9622f19c61681333d636b536dee00d4d5ebf32fe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957500"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskFolders = await graphClient.Me.Outlook.TaskFolders
    .Request()
    .GetAsync();

```