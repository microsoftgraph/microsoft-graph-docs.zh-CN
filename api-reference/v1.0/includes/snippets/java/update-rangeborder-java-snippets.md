---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e564ad6fbdfdc1f9b7400d36c934d8e01d638a2de7fecf2d5fc8768b076bea6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378253"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeBorder workbookRangeBorder = new WorkbookRangeBorder();
workbookRangeBorder.color = "color-value";
workbookRangeBorder.style = "style-value";
workbookRangeBorder.sideIndex = "sideIndex-value";
workbookRangeBorder.weight = "weight-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().borders("{sideIndex}")
    .buildRequest()
    .patch(workbookRangeBorder);

```