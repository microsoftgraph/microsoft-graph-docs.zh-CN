---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9eae1bccf9756469deaf7e5aa18905eebad2549
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209861"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("04487ee0-f4f6-4e7f-8999-facc5a30e232");

graphClient.identityProtection().riskyUsers()
    .dismiss(RiskyUserDismissParameterSet
        .newBuilder()
        .withUserIds(userIdsList)
        .build())
    .buildRequest()
    .post();

```