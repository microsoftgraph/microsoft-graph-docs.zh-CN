---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ec6adab112888ca3bae6128efdf0876c1206ef6
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Print.TaskDefinitions["92d72a3d-cad7-4809-8924-43833282b079"].Tasks
    .Request()
    .GetAsync();

```