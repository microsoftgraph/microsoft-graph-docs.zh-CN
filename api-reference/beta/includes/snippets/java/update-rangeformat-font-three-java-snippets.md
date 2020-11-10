---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 858921e6513820a0306f80a376d1893d28b37a91
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976078"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.underline = "Single";
workbookRangeFont.color = "#FFFFFF";
workbookRangeFont.size = 26d;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$C$1").format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```