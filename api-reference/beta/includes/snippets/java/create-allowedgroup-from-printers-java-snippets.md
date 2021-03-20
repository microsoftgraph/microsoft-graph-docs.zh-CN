---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97d819096a4da4d4ae19a043de5146ce27d7e064
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967988"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/groups/{id}"));

graphClient.print().shares("{id}").allowedGroups().references()
    .buildRequest()
    .post(group);

```