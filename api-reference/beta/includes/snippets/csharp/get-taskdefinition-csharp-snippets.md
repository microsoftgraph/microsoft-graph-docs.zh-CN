---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca6fee6b311f5742da4a429835799ab63510d6f0
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565309"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskDefinition = await graphClient.Print.TaskDefinitions["fab143fd-ee61-4358-8558-2c7dee953982"]
    .Request()
    .GetAsync();

```