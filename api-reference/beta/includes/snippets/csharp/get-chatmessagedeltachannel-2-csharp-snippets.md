---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9be94a2c59511563a3f1e2eed54e35e1d8df9913eafba64bc288c4444ad1afc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$skiptoken", "-FG3FPHv7HuyuazNLuy3eXlzQGbEjYLUsW9-pYkmXgn5KGsaOwrCoor2W23dGNNM1KtAX4AyvpFQNVsBgsEwUOX9lw8x9zDumgJy-C-UbjZLlZDQACyC9FyrVelZus9n.--rshdLwy_WBFJd8anPXJPbSUtUD7r3V4neB5tcrG58")
};

var delta = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Delta()
    .Request()
    .GetAsync();

```