---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac64b0201fb5df39ed7d3726c64540677ec238cf
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015144"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String name = "test5";

JsonElement reference = JsonParser.parseString("=Sheet1!$F$15:$N$27");

String comment = "Comment for the named item";

graphClient.me().drive().items("{id}").workbook().names()
    .add(name,reference,comment)
    .buildRequest()
    .post();

```