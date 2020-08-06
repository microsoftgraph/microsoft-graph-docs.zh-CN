---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c90c154f25e1b46a45a097bf96dc9ccea01f661e
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566127"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().conditionalAccess().policies("{id}")
    .buildRequest()
    .delete();

```