---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d078030ec9fc5f62838a4f88f51d894b1a7e14b4
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565896"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskTriggers = await graphClient.Print.Printers["{id}"].TaskTriggers
    .Request()
    .GetAsync();

```