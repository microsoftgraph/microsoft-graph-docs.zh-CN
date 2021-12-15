---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fe85842d061273ea52c7a087132e74f24f5d419
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526090"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String availability = "DoNotDisturb";

String activity = "DoNotDisturb";

Duration expirationDuration = DatatypeFactory.newInstance().newDuration("PT8H");

graphClient.users("fa8bf3dc-eca7-46b7-bad1-db199b62afc3").presence()
    .setUserPreferredPresence(PresenceSetUserPreferredPresenceParameterSet
        .newBuilder()
        .withAvailability(availability)
        .withActivity(activity)
        .withExpirationDuration(expirationDuration)
        .build())
    .buildRequest()
    .post();

```