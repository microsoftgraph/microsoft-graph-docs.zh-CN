---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a4dce138647fc2664000d68e34d955d470bec35
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223940"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AllowedValue allowedValue = new AllowedValue();
allowedValue.isActive = false;

graphClient.directory().customSecurityAttributeDefinitions("Engineering_Project").allowedValues("Alpine")
    .buildRequest()
    .patch(allowedValue);

```