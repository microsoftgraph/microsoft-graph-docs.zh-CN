---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b79ec9ed4e94e7b3773a91432898281a880e1ac2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980386"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTable workbookTable = new WorkbookTable();
workbookTable.name = "name-value";
workbookTable.showHeaders = true;
workbookTable.showTotals = true;
workbookTable.style = "style-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .buildRequest()
    .patch(workbookTable);

```