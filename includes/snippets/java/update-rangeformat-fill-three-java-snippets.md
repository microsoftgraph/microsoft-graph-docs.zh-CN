---
description: 自动生成的文件。 不修改
ms.openlocfilehash: baa61d97d1d31827299575dff7e57937eec44c2a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857365"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#0000FF";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range('$C$1').format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```