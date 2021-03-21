---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 570ca7713bf5eaeeb0520642d89bde738e60de81
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960846"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("04487ee0-f4f6-4e7f-8999-facc5a30e232");
userIdsList.add("13387ee0-f4f6-4e7f-8999-facc5120e345");

graphClient.riskyUsers()
    .dismiss(userIdsList)
    .buildRequest()
    .post();

```