---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a405ee425a7b8383db9a7e31fd5b5e7f4c31738
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984074"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#FF0000";

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$A$1")
        .build()).format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```