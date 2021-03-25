---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41bc28d2e14479c56f5d67afdfec19bbce6b5fb9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210302"
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