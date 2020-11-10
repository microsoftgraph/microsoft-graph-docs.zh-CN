---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3fec2a8b7718eff2c8344322e05989c183fc57e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963478"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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