---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b3b5d5dd0f690ebdc718d371121a04389f42a70
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610374"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hostedContents = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"].Replies["{chatMessage-id}"].HostedContents
    .Request()
    .GetAsync();

```