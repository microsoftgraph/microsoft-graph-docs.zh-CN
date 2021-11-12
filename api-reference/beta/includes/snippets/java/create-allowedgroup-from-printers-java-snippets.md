---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b80539449454dec7adc139f529c9d2924b6f906077091ac75961163b375850b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279266"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/groups/{id}"));

graphClient.print().shares("{id}").allowedGroups().references()
    .buildRequest()
    .post(group);

```