---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f48a51f629fa3a492189cd022c27c981dadec5e2c8a693ffaa80ff06d5d35ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237715"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.underline = "Single";
workbookRangeFont.color = "#FFFFFF";
workbookRangeFont.size = 26;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$C$1").format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```