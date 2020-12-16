---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f84f065d10102a5ff15c62c4899fc0f2433f0297
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692821"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
user.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/users/{id}"));

graphClient.print().shares("{id}").allowedUsers().references()
    .buildRequest()
    .post(user);

```