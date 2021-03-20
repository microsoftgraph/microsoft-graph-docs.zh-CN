---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34cf6e6b7b3e41c4e318b01fa7699f85b880af54
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970207"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .updateTiIndicators(TiIndicatorUpdateTiIndicatorsParameterSet
        .newBuilder()
        .withValue(valueList)
        .build())
    .buildRequest()
    .post();

```