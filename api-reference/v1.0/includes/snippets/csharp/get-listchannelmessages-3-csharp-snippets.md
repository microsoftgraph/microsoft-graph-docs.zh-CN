---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 004d2edb48c639eadbdc10f207fbe4e3dfa08ba6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314689"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Request()
    .Expand("replies")
    .Top(1)
    .GetAsync();

```