---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3b57717c2e5b4460b4b4acba562858dae09386e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983724"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableRow workbookTableRow = new WorkbookTableRow();
workbookTableRow.index = 99;
workbookTableRow.values = JsonParser.parseString("\"values-value\"");

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows("{index}")
    .buildRequest()
    .patch(workbookTableRow);

```