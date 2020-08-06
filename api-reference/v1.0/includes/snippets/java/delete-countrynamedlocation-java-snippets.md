---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d6eacb9cbdfbbce72401a3b3f5f9e5be4f29c15
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567165"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().conditionalAccess().namedLocations("1c4427fd-0885-4a3d-8b23-09a899ffa959")
    .buildRequest()
    .delete();

```