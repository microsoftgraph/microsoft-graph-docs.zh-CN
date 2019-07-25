---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4231696afa691226ff1690948be0bb39c98b5b87
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866017"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheetProtectionOptions options = new WorkbookWorksheetProtectionOptions();
options.allowFormatCells = true;
options.allowFormatColumns = true;
options.allowFormatRows = true;
options.allowInsertColumns = true;
options.allowInsertRows = true;
options.allowInsertHyperlinks = true;
options.allowDeleteColumns = true;
options.allowDeleteRows = true;
options.allowSort = true;
options.allowAutoFilter = true;
options.allowPivotTables = true;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").protection()
    .protect(options)
    .buildRequest()
    .post();

```