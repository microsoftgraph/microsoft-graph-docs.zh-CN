---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea0ac5176e1c6b12a980248a4ac67dbeee3e9e65cf8407fc1889a338925d64d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106005"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String name = "test5";

JsonElement reference = JsonParser.parseString("=Sheet1!$F$15:$N$27");

String comment = "Comment for the named item";

graphClient.me().drive().items("{id}").workbook().names()
    .add(WorkbookNamedItemAddParameterSet
        .newBuilder()
        .withName(name)
        .withReference(reference)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```