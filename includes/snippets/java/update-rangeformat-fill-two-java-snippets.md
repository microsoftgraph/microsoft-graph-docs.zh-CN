---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2cebfb3e08111f03da953a890c50928b980b6d3e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857360"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#00FF00";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range('$B$1').format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```