---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4a989092aae67a3885a0b27c3fa169c522d618e4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520384"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessageHostedContent = await graphClient.Chats["{id}"].Messages["{id}"].HostedContents["{id}"]
    .Request()
    .GetAsync();

```