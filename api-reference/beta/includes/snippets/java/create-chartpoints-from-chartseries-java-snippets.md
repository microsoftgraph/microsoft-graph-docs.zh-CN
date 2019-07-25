---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 28194d5a05f3a1db0e205cf915b5d8083a21a302
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863784"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartPoint workbookChartPoint = new WorkbookChartPoint();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{undefined}").points()
    .buildRequest()
    .post(workbookChartPoint);

```