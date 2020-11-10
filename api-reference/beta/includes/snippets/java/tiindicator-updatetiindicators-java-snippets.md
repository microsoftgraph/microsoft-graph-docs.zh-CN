---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd158c03914b318e48175db4a75fc89eed240e65
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971996"
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
TiIndicatorCollectionResponse tiIndicatorCollectionResponse = new TiIndicatorCollectionResponse();
tiIndicatorCollectionResponse.value = valueList;
TiIndicatorCollectionPage tiIndicatorCollectionPage = new TiIndicatorCollectionPage(tiIndicatorCollectionResponse, null);

graphClient.security().tiIndicators()
    .updateTiIndicators(valueList)
    .buildRequest()
    .post();

```