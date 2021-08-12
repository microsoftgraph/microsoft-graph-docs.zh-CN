---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b70535bfa7bbada18f4d98930cc1f84c58febe01391fdc69ca61b00a4edfa57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237711"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#FF0000";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$A$1").format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```