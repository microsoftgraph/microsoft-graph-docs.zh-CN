---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4eb2c57411b0cf9d249449ba7314860ab12d0b45
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].FilesFolder
    .Request()
    .GetAsync();

```