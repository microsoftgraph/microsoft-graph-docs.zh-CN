---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7773bbb4fc85d8e9638d610bb0022e55ff16b0bd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950486"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("29f270bb-4d23-4f68-8a57-dc73dc0d4caf");
userIdsList.add("20f91ec9-d140-4d90-9cd9-f618587a1471");

graphClient.riskyUsers()
    .confirmCompromised(userIdsList)
    .buildRequest()
    .post();

```