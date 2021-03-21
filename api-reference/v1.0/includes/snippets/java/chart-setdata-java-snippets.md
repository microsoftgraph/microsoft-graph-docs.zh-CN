---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33b5573d79834d20a0211687cbbfcb6a04938980
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980710"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

JsonElement sourceData = JsonParser.parseString("sourceData-value");

String seriesBy = "seriesBy-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .setData(WorkbookChartSetDataParameterSet
        .newBuilder()
        .withSourceData(sourceData)
        .withSeriesBy(seriesBy)
        .build())
    .buildRequest()
    .post();

```