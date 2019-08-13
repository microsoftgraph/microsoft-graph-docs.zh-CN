---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e1903ae6b1a29bde6c25ea4b8120885c08281745
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324767"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.underline = "Single";
workbookRangeFont.color = "#FFFFFF";
workbookRangeFont.size = 26;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range("$C$1").format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```