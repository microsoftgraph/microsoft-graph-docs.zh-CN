---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: c768c1c051621d92ad3ccf6e25a978fbc1eaf7f3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214335"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewInstanceDecisionItemCollectionPage decisions = graphClient.identityGovernance().accessReviews().definitions("60860cdd-fb4d-4054-91ba-444404f3baa6").instances("14444cdb-6a18-4c08-ba2c-48c02f0a0138").decisions()
    .buildRequest()
    .skip(0)
    .top(100)
    .get();

```