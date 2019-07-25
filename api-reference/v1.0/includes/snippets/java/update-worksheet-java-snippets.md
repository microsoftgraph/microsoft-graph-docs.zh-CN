---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 39085a925910c45a540cfa88a2222a6ce02db620
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884225"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheet workbookWorksheet = new WorkbookWorksheet();
workbookWorksheet.position = 99;
workbookWorksheet.name = "name-value";
workbookWorksheet.visibility = "visibility-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .buildRequest()
    .patch(workbookWorksheet);

```