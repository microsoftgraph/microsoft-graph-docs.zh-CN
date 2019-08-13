---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 02a90afa3cc5bfcab3f97a3e9eedf5496bc11d1b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324758"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.italic = true;
workbookRangeFont.size = 26;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range("$B$1").format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```