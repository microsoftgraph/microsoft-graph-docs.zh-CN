---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0c1608e92131bb438032a8ebdcedb5fc761a3a91
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882048"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartAxis workbookChartAxis = new WorkbookChartAxis();
Json majorUnit = new Json();
workbookChartAxis.majorUnit = majorUnit;
Json maximum = new Json();
workbookChartAxis.maximum = maximum;
Json minimum = new Json();
workbookChartAxis.minimum = minimum;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis()
    .buildRequest()
    .patch(workbookChartAxis);

```