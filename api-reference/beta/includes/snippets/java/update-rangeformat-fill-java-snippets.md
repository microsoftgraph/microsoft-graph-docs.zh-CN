---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4662cab216d0c6ab99fedeb083e56fe77776849457c336c04c1b40285b5befdf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106278"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#FF0000";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$A$1")
        .build()).format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```