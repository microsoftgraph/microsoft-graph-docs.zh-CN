---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad0fa61e9916d2e6f02dd2a1584293a8cf50adf1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969270"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}")
    .archive(TeamArchiveParameterSet
        .newBuilder()
        .withShouldSetSpoSiteReadOnlyForMembers(null)
        .build())
    .buildRequest()
    .post();

```