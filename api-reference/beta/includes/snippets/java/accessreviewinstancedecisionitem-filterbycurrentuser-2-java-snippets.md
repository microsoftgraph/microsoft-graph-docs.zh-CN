---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9156f7f0bcc2f55c52363f8cdc766ff80112d442
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853413"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItemFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().accessReviews().definitions("0185aab8-9a7e-44b5-ae36-41b923c3bf87").instances("1234aab8-9a7e-5678-ae36-41b923c3bf87").stages("9458f255-dff2-4d86-9a05-69438f49d7f8").decisions()
    .filterByCurrentUser(AccessReviewInstanceDecisionItemFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('reviewer')
        .build())
    .buildRequest()
    .get();

```