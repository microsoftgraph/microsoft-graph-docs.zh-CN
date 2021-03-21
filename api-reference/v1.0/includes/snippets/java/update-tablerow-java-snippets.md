---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40298dacb32f5d7817f0a39c9980dec3f35a7ce8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977812"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableRow workbookTableRow = new WorkbookTableRow();
workbookTableRow.index = 99;
workbookTableRow.values = JsonParser.parseString("\"values-value\"");

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows("{index}")
    .buildRequest()
    .patch(workbookTableRow);

```