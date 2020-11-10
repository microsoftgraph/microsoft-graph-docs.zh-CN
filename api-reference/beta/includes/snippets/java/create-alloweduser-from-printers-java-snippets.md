---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ac809a75aab826cd1c5f17e1877c64fa50e31c9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968413"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUserIdentity printUserIdentity = new PrintUserIdentity();
printUserIdentity.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/users/{id}"));

graphClient.print().shares("{id}").allowedUsers().references()
    .buildRequest()
    .post(printUserIdentity);

```