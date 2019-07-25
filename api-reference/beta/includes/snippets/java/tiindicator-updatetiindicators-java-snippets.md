---
description: 自动生成的文件。 不修改
ms.openlocfilehash: db136d7be4cfb45c1af4851e3a44406a3c8fea84
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868146"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<TiIndicator> valueList = new LinkedList<TiIndicator>();
TiIndicator value = new TiIndicator();
value.id = "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4";
value.additionalInformation = "mytest";

valueList.add(value);
TiIndicator value1 = new TiIndicator();
value1.id = "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e";
value1.additionalInformation = "test again";

valueList.add(value1);

graphClient.security().tiIndicators()
    .updateTiIndicators(valueList)
    .buildRequest()
    .post();

```