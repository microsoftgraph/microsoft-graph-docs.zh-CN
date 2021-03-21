---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b297dd8d2faf46c07692ab38147a0381e548aa9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957205"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var names = await graphClient.Me.Profile.Names
    .Request()
    .GetAsync();

```