---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 84d2cb8da772e3875c2a4777c97ba4b08e6d0e99
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214743"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewInstanceCollectionPage instances = graphClient.identityGovernance().accessReviews().definitions("60860cdd-fb4d-4054-91ba-f75e04f34444").instances()
    .buildRequest()
    .skip(0)
    .top(100)
    .get();

```