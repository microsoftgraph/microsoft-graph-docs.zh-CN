---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de5414ab68ebd0bb60b430bea4d675f94f0cf21f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805776"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members
    .Request()
    .GetAsync();

```