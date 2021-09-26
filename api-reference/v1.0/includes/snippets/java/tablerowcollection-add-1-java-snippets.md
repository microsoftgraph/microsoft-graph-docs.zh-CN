---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c895ec0fec2f226e64d8b2f7d1442c46dfcee1ab
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763864"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "respond-async"));
requestOptions.add(new HeaderOption("Workbook-Session-Id", "{Workbook-Session-Id}"));

WorkbookTableRow workbookTableRow = new WorkbookTableRow();
workbookTableRow.values = JsonParser.parseString("\"[\r\n    [1, 2, 3],\r\n    [4, 5, 6]\r\n  ]\"");

graphClient.me().drive().items("01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ").workbook().tables("Table1").rows()
    .buildRequest( requestOptions )
    .post(workbookTableRow);

```