---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 507c642e0a1db787e2951475e27959e354e589713e925d2a896fa94a0f55330f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161794"
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