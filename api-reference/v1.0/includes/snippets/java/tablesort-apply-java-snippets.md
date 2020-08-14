---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a87ddf1018dfc649e20140da1f3da498413dd75
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402116"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<WorkbookSortField> fieldsList = new LinkedList<WorkbookSortField>();
WorkbookSortField fields = new WorkbookSortField();
fields.key = 99;
fields.sortOn = "sortOn-value";
fields.ascending = true;
fields.color = "color-value";
fields.dataOption = "dataOption-value";
WorkbookIcon icon = new WorkbookIcon();
icon.set = "set-value";
icon.index = 99;
fields.icon = icon;

fieldsList.add(fields);

boolean matchCase = true;

String method = "method-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").sort()
    .apply(fieldsList,matchCase,method)
    .buildRequest()
    .post();

```