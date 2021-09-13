---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0443d75173adfc97a4ba3e48473ac04cd6d16af3d624f54677853414e0c73120
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163864"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItemFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().accessReviews().definitions("1234ea1c-8d12-457b-1234-a37dc59e54e0").instances("7070ea1c-8d12-457b-bd35-a37dc59e54e0").decisions()
    .filterByCurrentUser(AccessReviewInstanceDecisionItemFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('reviewer')
        .build())
    .buildRequest()
    .get();

```