---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 398f2c7a2fc8b852e8e45bd947c737c4cb9ca5ec
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966582"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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