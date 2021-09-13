---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6ccced3f3498dc24932d2c2c5ad64a3added9bdfc590aaac500e54718a39679
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902300"
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