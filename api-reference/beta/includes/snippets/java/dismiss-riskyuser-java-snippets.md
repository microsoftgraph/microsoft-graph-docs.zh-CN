---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a15922bb9692ab7b0593c283022d7fd76ecaf2c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975888"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("04487ee0-f4f6-4e7f-8999-facc5a30e232");

graphClient.identityProtection().riskyUsers()
    .dismiss(userIdsList)
    .buildRequest()
    .post();

```