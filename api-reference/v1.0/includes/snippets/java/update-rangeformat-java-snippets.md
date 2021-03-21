---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1156152b1c882a2a2913115e354905c884f53d8b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976392"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = new WorkbookRangeFormat();
workbookRangeFormat.columnWidth = 135d;
workbookRangeFormat.verticalAlignment = "Top";
workbookRangeFormat.rowHeight = 49d;
workbookRangeFormat.wrapText = false;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$A$1")
        .build()).format()
    .buildRequest()
    .patch(workbookRangeFormat);

```