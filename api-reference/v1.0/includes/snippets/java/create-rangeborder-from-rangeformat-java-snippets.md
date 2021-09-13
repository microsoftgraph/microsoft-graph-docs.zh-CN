---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb6dbe9e04612104771454695854029a9be082757972041614585247dda72a0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277210"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeBorder workbookRangeBorder = new WorkbookRangeBorder();
workbookRangeBorder.id = "id-value";
workbookRangeBorder.color = "color-value";
workbookRangeBorder.style = "style-value";
workbookRangeBorder.sideIndex = "sideIndex-value";
workbookRangeBorder.weight = "weight-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().borders()
    .buildRequest()
    .post(workbookRangeBorder);

```