---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1038d23372450ed2608e843c91cce33c523f60efaaaad442f9407c0d93795f9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903641"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> valueList = new LinkedList<String>();
valueList.add("externalId-value1");
valueList.add("externalId-value2");

graphClient.security().tiIndicators()
    .deleteTiIndicatorsByExternalId(TiIndicatorDeleteTiIndicatorsByExternalIdParameterSet
        .newBuilder()
        .withValue(valueList)
        .build())
    .buildRequest()
    .post();

```