---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a25b1e3a4549a67b240026bd07b01dc861b6a72
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.TaskDefinitions["4c6a0f26-8e5d-4bf6-91e6-4a5731adec19"]
    .Request()
    .DeleteAsync();

```