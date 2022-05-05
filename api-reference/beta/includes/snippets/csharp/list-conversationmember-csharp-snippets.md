---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d7a8695efc275573e72f68f83c394194b4544bd
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212874"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedMembers = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].SharedWithTeams["{sharedWithChannelTeamInfo-id}"].AllowedMembers
    .Request()
    .GetAsync();

```