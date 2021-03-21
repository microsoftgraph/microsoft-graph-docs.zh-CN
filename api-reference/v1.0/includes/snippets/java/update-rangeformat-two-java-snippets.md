---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f9e59ff3116d0e992d7cae1f3b4f27f9e9980ee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978225"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = new WorkbookRangeFormat();
workbookRangeFormat.columnWidth = 135d;
workbookRangeFormat.horizontalAlignment = "Center";
workbookRangeFormat.verticalAlignment = "Center";
workbookRangeFormat.rowHeight = 49d;
workbookRangeFormat.wrapText = false;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$B$1")
        .build()).format()
    .buildRequest()
    .patch(workbookRangeFormat);

```