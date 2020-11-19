---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: f7c27a9e8abbbad1f3b88fe4422aebded51d6cf7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221921"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewInstanceDecisionItemCollectionPage decisions = graphClient.me().pendingAccessReviewInstances("70a68410-67f3-4d4c-b946-6989e050be19").decisions()
    .buildRequest()
    .skip(0)
    .top(100)
    .get();

```