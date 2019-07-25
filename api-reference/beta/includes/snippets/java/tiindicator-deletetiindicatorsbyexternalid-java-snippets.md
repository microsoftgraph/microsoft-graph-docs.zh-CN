---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8dc7c7c3804461f0b7fcc83ae770c0adc7c3aa63
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868240"
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