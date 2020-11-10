---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dc7c7c3804461f0b7fcc83ae770c0adc7c3aa63
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977729"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> valueList = new LinkedList<String>();
valueList.add("externalId-value1");
valueList.add("externalId-value2");

graphClient.security().tiIndicators()
    .deleteTiIndicatorsByExternalId(valueList)
    .buildRequest()
    .post();

```