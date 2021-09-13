---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c65d128b83c05e9a2cac1c4e7163d6548700a30e1682f8d18e9354333d9afb0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409762"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "ColumnStacked";

JsonElement sourceData = JsonParser.parseString("A1:B1");

String seriesBy = "Auto";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts()
    .add(WorkbookChartAddParameterSet
        .newBuilder()
        .withType(type)
        .withSourceData(sourceData)
        .withSeriesBy(seriesBy)
        .build())
    .buildRequest()
    .post();

```