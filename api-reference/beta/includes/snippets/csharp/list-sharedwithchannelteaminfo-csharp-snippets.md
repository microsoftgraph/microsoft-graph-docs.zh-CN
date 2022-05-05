---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d83601a0afe3d890c142650399b09c98cbe1614
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212780"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedWithTeams = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].SharedWithTeams
    .Request()
    .GetAsync();

```