---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6f4f19c63fe9d7851905367e88a35f65adb07983e50e60319fc38cb2d80da02
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163056"
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