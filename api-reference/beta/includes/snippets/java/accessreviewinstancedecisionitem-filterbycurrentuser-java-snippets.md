---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c36d36cbd8d186e7b03acea48dc3b65ed975f04552a1fbe4b1317b2669dd69a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902665"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItemFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().accessReviews().definitions("0185aab8-9a7e-44b5-ae36-41b923c3bf87").instances("1234aab8-9a7e-5678-ae36-41b923c3bf87").decisions()
    .filterByCurrentUser(AccessReviewInstanceDecisionItemFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('reviewer')
        .build())
    .buildRequest()
    .get();

```