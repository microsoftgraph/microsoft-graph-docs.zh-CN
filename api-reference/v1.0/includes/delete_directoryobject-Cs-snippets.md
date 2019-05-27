---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dee8989e645d157a0e173e9ae2330902266fb672
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459333"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryObjects["{id}"]
    .Request()
    .DeleteAsync();

```