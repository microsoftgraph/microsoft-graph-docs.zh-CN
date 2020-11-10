---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 495452d16cbfbecd640057bbd512bdace1635eec
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976073"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#00FF00";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$B$1").format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```