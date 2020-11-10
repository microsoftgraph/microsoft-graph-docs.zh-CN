---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7312590a6834e99d8f28909279a27013a4ba15de
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958387"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartSeries workbookChartSeries = new WorkbookChartSeries();
workbookChartSeries.name = "name-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{undefined}")
    .buildRequest()
    .patch(workbookChartSeries);

```