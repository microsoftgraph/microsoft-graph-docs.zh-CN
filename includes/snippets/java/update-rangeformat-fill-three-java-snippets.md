---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffca07235312087c81bad6ef9de8c5dda2dcd34fd4c522ea9f6172b80607b55d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237712"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#0000FF";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$C$1").format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```