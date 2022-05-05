---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 909af2622e17326b9cbd1f146298a3d677eab9ba
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedWithChannelTeamInfo = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].SharedWithTeams["{sharedWithChannelTeamInfo-id}"]
    .Request()
    .GetAsync();

```