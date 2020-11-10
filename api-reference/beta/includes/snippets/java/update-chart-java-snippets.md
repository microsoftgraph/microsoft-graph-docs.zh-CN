---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 472c564ccdeb1f988ded5ae323df0e230d6ffadf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958947"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChart workbookChart = new WorkbookChart();
workbookChart.height = 99d;
workbookChart.left = 99d;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .buildRequest()
    .patch(workbookChart);

```