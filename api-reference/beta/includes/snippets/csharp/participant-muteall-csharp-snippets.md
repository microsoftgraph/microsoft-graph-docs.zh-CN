---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d6d4477c2ef6ceadb5f7cbc2b7872f561fdefa3c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500679"
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