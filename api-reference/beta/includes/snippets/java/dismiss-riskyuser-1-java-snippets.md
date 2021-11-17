---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd473ba54f5c5d61985505a08fdf5d4ae2b5d9621158c7e062c1e4c2ecdb93f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903076"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("04487ee0-f4f6-4e7f-8999-facc5a30e232");
userIdsList.add("13387ee0-f4f6-4e7f-8999-facc5120e345");

graphClient.riskyUsers()
    .dismiss(RiskyUserDismissParameterSet
        .newBuilder()
        .withUserIds(userIdsList)
        .build())
    .buildRequest()
    .post();

```