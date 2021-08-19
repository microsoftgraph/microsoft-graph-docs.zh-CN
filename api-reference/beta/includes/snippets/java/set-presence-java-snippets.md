---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f98c5c6108fab5b76b093de30e856ed8fc464796dcc7309d5b4cf8697424a7af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220083"
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