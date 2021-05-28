---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d7c89428426579c0ba7060d04934ed7358a0323
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610375"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hostedContents = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"].HostedContents
    .Request()
    .GetAsync();

```