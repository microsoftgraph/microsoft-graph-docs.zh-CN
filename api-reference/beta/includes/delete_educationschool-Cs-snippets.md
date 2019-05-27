---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0933b3bcf9bdabc4026ba9a9c4c05d530e799dda
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438397"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["10002"]
    .Request()
    .DeleteAsync();

```