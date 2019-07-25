---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5f546d51ce5c527a9a334a6d22823471e2df3776
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891378"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartPoint workbookChartPoint = new WorkbookChartPoint();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{series-id}").points()
    .buildRequest()
    .post(workbookChartPoint);

```