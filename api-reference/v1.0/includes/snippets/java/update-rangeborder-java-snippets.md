---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41b7b2df298736f03a29a237858a0e0ae0f813d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967848"
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