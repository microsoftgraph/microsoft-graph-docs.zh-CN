---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 570ca7713bf5eaeeb0520642d89bde738e60de81
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871008"
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