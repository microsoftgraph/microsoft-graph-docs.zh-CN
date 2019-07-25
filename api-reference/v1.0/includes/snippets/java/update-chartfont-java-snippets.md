---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d4fe98762d7d7de1b1ffffeb5c21150724dd83b0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890401"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartFont workbookChartFont = new WorkbookChartFont();
workbookChartFont.bold = true;
workbookChartFont.color = "color-value";
workbookChartFont.italic = true;
workbookChartFont.name = "name-value";
workbookChartFont.size = 99;
workbookChartFont.underline = "underline-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis().format().font()
    .buildRequest()
    .patch(workbookChartFont);

```