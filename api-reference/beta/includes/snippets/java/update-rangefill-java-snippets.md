---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a331a01195b49d2ccf7e2e21f955802a27d336e9d8cfd842342dd9b35bfd61dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274327"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "color-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```