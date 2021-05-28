---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee42edf6d69423321f23be2188eecee48f0e4941
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"].Replies["{chatMessage-id}"]
    .Request()
    .GetAsync();

```