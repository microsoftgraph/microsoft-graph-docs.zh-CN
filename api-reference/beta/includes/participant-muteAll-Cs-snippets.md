---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d6d4477c2ef6ceadb5f7cbc2b7872f561fdefa3c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = new List<String>()
{
    ""
};

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"].Participants
    .MuteAll(participants,clientContext)
    .Request()
    .PostAsync();

```