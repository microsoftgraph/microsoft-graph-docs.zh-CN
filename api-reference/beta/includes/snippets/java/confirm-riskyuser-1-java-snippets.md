---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9d4382e0771ad9bc3c9876d11204dafbcf31e1f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208753"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("29f270bb-4d23-4f68-8a57-dc73dc0d4caf");
userIdsList.add("20f91ec9-d140-4d90-9cd9-f618587a1471");

graphClient.riskyUsers()
    .confirmCompromised(RiskyUserConfirmCompromisedParameterSet
        .newBuilder()
        .withUserIds(userIdsList)
        .build())
    .buildRequest()
    .post();

```