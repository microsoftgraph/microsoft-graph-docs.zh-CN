---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 009a681d9a002d71305336a650fe1ef479335d4f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892005"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = new WorkbookRangeFormat();
workbookRangeFormat.columnWidth = 135;
workbookRangeFormat.horizontalAlignment = "Right";
workbookRangeFormat.verticalAlignment = "Top";
workbookRangeFormat.rowHeight = 49;
workbookRangeFormat.wrapText = false;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range('$C$1').format()
    .buildRequest()
    .patch(workbookRangeFormat);

```