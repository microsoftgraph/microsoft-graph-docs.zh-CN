---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8171ac8e455c7c98737d045194b2fec50ecc58bf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971856"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/groups/{groupId}"));

graphClient.print().shares("{printerShareId}").allowedGroups().references()
    .buildRequest()
    .post(group);

```