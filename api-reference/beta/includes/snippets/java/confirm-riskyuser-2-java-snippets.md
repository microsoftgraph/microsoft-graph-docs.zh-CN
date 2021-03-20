---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50b64cdc27daf5a958a61b147dbd38b2d449f937
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950499"
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