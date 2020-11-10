---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50b64cdc27daf5a958a61b147dbd38b2d449f937
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970940"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("29f270bb-4d23-4f68-8a57-dc73dc0d4caf");

graphClient.identityProtection().riskyUsers()
    .confirmCompromised(userIdsList)
    .buildRequest()
    .post();

```