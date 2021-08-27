---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb0c19ec3c162f2e98d326f893f964b867a84b872314f30f84796dce1bc64b8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"].Replies
    .Request()
    .GetAsync();

```