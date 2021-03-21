---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b03ce50ecf09e1b208e7f5345742a8208791019
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974676"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

int index = 3;

LinkedList<JsonElement> valuesList = new LinkedList<JsonElement>();
JsonElement values = new JsonObject();

valuesList.add(values);

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .add(WorkbookTableColumnAddParameterSet
        .newBuilder()
        .withIndex(index)
        .withValues(values)
        .withName(null)
        .build())
    .buildRequest()
    .post();

```