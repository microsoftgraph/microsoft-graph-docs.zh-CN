---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ce5890d07c40d8292d0ae1264979150760d4d88
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567127"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NamedLocation namedLocation = graphClient.identity().conditionalAccess().namedLocations("1c4427fd-0885-4a3d-8b23-09a899ffa959")
    .buildRequest()
    .get();

```