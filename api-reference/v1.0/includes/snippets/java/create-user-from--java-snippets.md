---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0665acfde880efff67e7b4348e9f94e14c3359ace5e110daff42f6a8612fd351
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218380"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
user.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/users/{userId}"));

graphClient.print().shares("{printerShareId}").allowedUsers().references()
    .buildRequest()
    .post(user);

```