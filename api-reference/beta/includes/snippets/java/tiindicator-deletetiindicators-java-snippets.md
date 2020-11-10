---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b07fda38e2c21dc656fdf57eb5a26f8df9e8d2d2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977750"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> valueList = new LinkedList<String>();
valueList.add("id-value1");
valueList.add("id-value2");

graphClient.security().tiIndicators()
    .deleteTiIndicators(valueList)
    .buildRequest()
    .post();

```