---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 259990ecc632f46d65d5cf7f96bad6ab19d18202
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437340"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["ba9a3254-9f18-4209-aeb3-9e42a35b5be4"]
    .Request()
    .DeleteAsync();

```