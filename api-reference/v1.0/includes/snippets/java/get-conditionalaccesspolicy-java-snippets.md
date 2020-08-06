---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 402030db21edccab5878a61a2fe877aee9f71c8f
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566094"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicy conditionalAccessPolicy = graphClient.identity().conditionalAccess().policies("{id}")
    .buildRequest()
    .get();

```