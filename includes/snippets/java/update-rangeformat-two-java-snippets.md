---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2ba425200b0261f936981f005884d0b8327e80a20c5ed62a315d59bc22aab25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237719"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = new WorkbookRangeFormat();
workbookRangeFormat.columnWidth = 135;
workbookRangeFormat.horizontalAlignment = "Center";
workbookRangeFormat.verticalAlignment = "Center";
workbookRangeFormat.rowHeight = 49;
workbookRangeFormat.wrapText = false;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$B$1").format()
    .buildRequest()
    .patch(workbookRangeFormat);

```