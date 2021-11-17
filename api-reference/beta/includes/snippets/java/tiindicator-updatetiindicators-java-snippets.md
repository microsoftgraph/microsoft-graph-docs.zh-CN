---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d592d3db20a40b1476f8706492b7a092ba71df95903405895fe9cf855ab01e2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220187"
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