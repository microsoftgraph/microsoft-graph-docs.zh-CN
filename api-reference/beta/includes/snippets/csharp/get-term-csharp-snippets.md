---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 963c724f4c33bd1636aa46607663e261315c8db2
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329926"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.TermStore.Sets["{setId}"].Children
    .Request()
    .GetAsync();

```