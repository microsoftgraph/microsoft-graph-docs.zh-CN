---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9e942b40ff6c77643e26dbf4e3837b85ce6a082d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874241"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#FF0000";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range('$A$1').format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```