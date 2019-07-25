---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c7519399306da17cc126870c0ff4623748514159
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890232"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookNamedItem workbookNamedItem = new WorkbookNamedItem();
workbookNamedItem.type = "type-value";
workbookNamedItem.scope = "scope-value";
workbookNamedItem.comment = "comment-value";
Json value = new Json();
workbookNamedItem.value = value;
workbookNamedItem.visible = true;

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .buildRequest()
    .patch(workbookNamedItem);

```