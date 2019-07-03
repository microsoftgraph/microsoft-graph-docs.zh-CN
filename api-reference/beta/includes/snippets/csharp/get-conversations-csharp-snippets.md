---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b60d6146a22b612e7f1093ad1dbdbc6ca304fec4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500698"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversations = await graphClient.Groups["{id}"].Conversations
    .Request()
    .GetAsync();

```