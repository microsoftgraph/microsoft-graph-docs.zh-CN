---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce7043a92abaca4645b870865222423517746100
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984086"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.bold = true;
workbookRangeFont.color = "color-value";
workbookRangeFont.italic = true;
workbookRangeFont.name = "name-value";
workbookRangeFont.size = 99d;
workbookRangeFont.underline = "underline-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```