---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3b7a8cfd506c7de30f4527d8f6df638824c6ec3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976072"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = new WorkbookRangeFormat();
workbookRangeFormat.columnWidth = 135d;
workbookRangeFormat.horizontalAlignment = "Center";
workbookRangeFormat.verticalAlignment = "Center";
workbookRangeFormat.rowHeight = 49d;
workbookRangeFormat.wrapText = false;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$B$1").format()
    .buildRequest()
    .patch(workbookRangeFormat);

```