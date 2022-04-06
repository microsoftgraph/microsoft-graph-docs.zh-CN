---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 828a115dbeb4a0f1c20efec55f16b134b6a3a1af
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528166"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$skiptoken", "-FG3FPHv7HuyuazNLuy3eXlzQGbEjYLUsW9-pYkmXgn5KGsaOwrCoor2W23dGNNM1KtAX4AyvpFQNVsBgsEwUOX9lw8x9zDumgJy-C-UbjZLlZDQACyC9FyrVelZus9n.--rshdLwy_WBFJd8anPXJPbSUtUD7r3V4neB5tcrG58")
};

var delta = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Delta()
    .Request( queryOptions )
    .GetAsync();

```