---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4338380119c5b2f2f5a1c99ff82aa53cd27b878a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982954"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableColumn workbookTableColumn = new WorkbookTableColumn();
workbookTableColumn.id = 99;
workbookTableColumn.name = "name-value";
workbookTableColumn.index = 99;
workbookTableColumn.values = JsonParser.parseString("\"values-value\"");

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .buildRequest()
    .post(workbookTableColumn);

```