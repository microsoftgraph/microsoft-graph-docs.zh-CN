---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 669926c48c81d86dbfb0fd0985262731f7202fbc
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854162"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewStageFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().accessReviews().definitions("08531375-eff6-4e21-b1a8-de0eb37ec913").instances("86889534-b102-4226-bfce-0c2aeee845df").stages()
    .filterByCurrentUser(AccessReviewStageFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('reviewer')
        .build())
    .buildRequest()
    .get();

```