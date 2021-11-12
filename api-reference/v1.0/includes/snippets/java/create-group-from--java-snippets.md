---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d68c84577b9d034df81f78447fbae7eb5227a98bffa89bdd9c10edf637c29e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378726"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/groups/{groupId}"));

graphClient.print().shares("{printerShareId}").allowedGroups().references()
    .buildRequest()
    .post(group);

```