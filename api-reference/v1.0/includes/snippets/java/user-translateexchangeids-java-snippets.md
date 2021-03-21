---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee8cdb2c2b4400b2390a435df1c44fea7ff1eb1c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983508"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> inputIdsList = new LinkedList<String>();
inputIdsList.add("{rest-formatted-id-1}");
inputIdsList.add("{rest-formatted-id-2}");

ExchangeIdFormat sourceIdType = ExchangeIdFormat.REST_ID;

ExchangeIdFormat targetIdType = ExchangeIdFormat.REST_IMMUTABLE_ENTRY_ID;

graphClient.me()
    .translateExchangeIds(UserTranslateExchangeIdsParameterSet
        .newBuilder()
        .withInputIds(inputIdsList)
        .withTargetIdType(targetIdType)
        .withSourceIdType(sourceIdType)
        .build())
    .buildRequest()
    .post();

```