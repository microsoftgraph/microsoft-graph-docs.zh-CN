---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9970017e241b150daff26a5bb4373738e207e2c7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886163"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartDataLabels workbookChartDataLabels = new WorkbookChartDataLabels();
workbookChartDataLabels.position = "position-value";
workbookChartDataLabels.showValue = true;
workbookChartDataLabels.showSeriesName = true;
workbookChartDataLabels.showCategoryName = true;
workbookChartDataLabels.showLegendKey = true;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").dataLabels()
    .buildRequest()
    .patch(workbookChartDataLabels);

```