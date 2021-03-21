---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 979d041e8f66fa0f7a87a6032f12081f83c14d7c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971543"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.bold = true;
workbookRangeFont.color = "#4B180E";
workbookRangeFont.size = 26d;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$A$1")
        .build()).format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```