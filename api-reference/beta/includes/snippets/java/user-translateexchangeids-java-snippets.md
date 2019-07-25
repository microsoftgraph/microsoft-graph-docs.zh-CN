---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c17ed789e4742c08287a9b44d5dfefbe24eb3c8d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866690"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> inputIdsList = new LinkedList<String>();
inputIdsList.add("{rest-formatted-id-1}");
inputIdsList.add("{rest-formatted-id-2}");

ExchangeIdFormat sourceIdType = ExchangeIdFormat.REST_ID;

ExchangeIdFormat targetIdType = ExchangeIdFormat.REST_IMMUTABLE_ENTRY_ID;

graphClient.me()
    .translateExchangeIds(inputIdsList,targetIdType,sourceIdType)
    .buildRequest()
    .post();

```