---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d79d1a8be528fcbb1ec502fedbb015b7b093b16a
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514026"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String sessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87";

String availability = "Available";

String activity = "Available";

Duration expirationDuration = DatatypeFactory.newInstance().newDuration("PT1H");

graphClient.users("fa8bf3dc-eca7-46b7-bad1-db199b62afc3").presence()
    .setPresence(PresenceSetPresenceParameterSet
        .newBuilder()
        .withSessionId(sessionId)
        .withAvailability(availability)
        .withActivity(activity)
        .withExpirationDuration(expirationDuration)
        .build())
    .buildRequest()
    .post();

```