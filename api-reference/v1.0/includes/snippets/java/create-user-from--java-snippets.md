---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00cd24ee0d635e81a602d2531f5bdf829d2129da
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969897"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
user.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/users/{userId}"));

graphClient.print().shares("{printerShareId}").allowedUsers().references()
    .buildRequest()
    .post(user);

```