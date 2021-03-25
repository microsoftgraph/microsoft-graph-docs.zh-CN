---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5a9e1dcbedb4fca7a1b3b76638c73bb8a2dc9da
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210943"
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