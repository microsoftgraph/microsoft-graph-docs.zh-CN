---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 641e7413b4182c944bdc212fcf71d71ba28f6a04
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324756"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = new WorkbookRangeFormat();
workbookRangeFormat.columnWidth = 135;
workbookRangeFormat.horizontalAlignment = "Center";
workbookRangeFormat.verticalAlignment = "Center";
workbookRangeFormat.rowHeight = 49;
workbookRangeFormat.wrapText = false;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range("$B$1").format()
    .buildRequest()
    .patch(workbookRangeFormat);

```