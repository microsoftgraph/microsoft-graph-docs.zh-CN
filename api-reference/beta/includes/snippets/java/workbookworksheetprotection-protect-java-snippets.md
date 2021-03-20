---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e918edfbef1ba9a3cb05b5bff3eb535ddf9dfbbd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976083"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .protect(WorkbookWorksheetProtectionProtectParameterSet
        .newBuilder()
        .withOptions(options)
        .build())
    .buildRequest()
    .post();

```