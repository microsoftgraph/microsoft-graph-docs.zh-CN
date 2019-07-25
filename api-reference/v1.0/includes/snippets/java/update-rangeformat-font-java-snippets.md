---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ffa02dbb72a9e0e21252d17a9a310fc82b6ad54a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891998"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.bold = true;
workbookRangeFont.color = "#4B180E";
workbookRangeFont.size = 26;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range('$A$1').format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```