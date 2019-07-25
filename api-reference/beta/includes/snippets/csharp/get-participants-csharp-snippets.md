---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e7f12dbc19a85b50c58ddcb69e24b7ad05edec1a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708916"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = await graphClient.App.Calls["57DAB8B1894C409AB240BD8BEAE78896"].Participants
    .Request()
    .Header("Authorization","Bearer <TOKEN>")
    .GetAsync();

```