---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e15b896d94e34accbf59506138eb154fb7251ac4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438038"
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