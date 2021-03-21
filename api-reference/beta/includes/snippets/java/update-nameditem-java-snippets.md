---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fcfa5aec6b563ef96df31213a72ac68189ac4f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984084"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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