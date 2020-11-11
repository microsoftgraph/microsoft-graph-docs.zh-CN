---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7c3db5c1de9b6dff6c2fca306c6502b2bb3e9f3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983867"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookNamedItem workbookNamedItem = new WorkbookNamedItem();
workbookNamedItem.type = "type-value";
workbookNamedItem.scope = "scope-value";
workbookNamedItem.comment = "comment-value";
JsonElement value = new JsonObject();
workbookNamedItem.value = value;
workbookNamedItem.visible = true;

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .buildRequest()
    .patch(workbookNamedItem);

```