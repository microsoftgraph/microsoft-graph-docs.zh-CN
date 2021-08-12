---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f75fc451bc7280a8bd40c13d587724f980127c2dccd0254a14d51032df8dd7e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237714"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.bold = true;
workbookRangeFont.color = "#4B180E";
workbookRangeFont.size = 26;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$A$1").format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```