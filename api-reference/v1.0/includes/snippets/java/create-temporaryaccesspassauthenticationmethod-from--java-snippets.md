---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e15b896d94e34accbf59506138eb154fb7251ac4
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093337"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethod temporaryAccessPassAuthenticationMethod = new TemporaryAccessPassAuthenticationMethod();
temporaryAccessPassAuthenticationMethod.startDateTime = OffsetDateTimeSerializer.deserialize("2022-06-05T00:00:00Z");
temporaryAccessPassAuthenticationMethod.lifetimeInMinutes = 60;
temporaryAccessPassAuthenticationMethod.isUsableOnce = false;

graphClient.users("071cc716-8147-4397-a5ba-b2105951cc0b").authentication().temporaryAccessPassMethods()
    .buildRequest()
    .post(temporaryAccessPassAuthenticationMethod);

```