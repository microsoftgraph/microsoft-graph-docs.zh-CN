---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90fda57b2ca3bf40b2eb31104e61d01bb1e38263
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cases = await graphClient.Compliance.Ediscovery.Cases
    .Request()
    .GetAsync();

```