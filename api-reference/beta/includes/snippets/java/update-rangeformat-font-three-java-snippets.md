---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6d663ac9e0d6618ceb20e7423cdbb3d058a156b4598f28c9d78b2350413dc0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903751"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.underline = "Single";
workbookRangeFont.color = "#FFFFFF";
workbookRangeFont.size = 26d;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$C$1")
        .build()).format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```