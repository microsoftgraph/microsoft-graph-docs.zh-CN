---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a2f6b124d2c18313fe86a9602a5bfdaebdeb917
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Tabs
    .Request()
    .Expand("teamsApp")
    .GetAsync();

```