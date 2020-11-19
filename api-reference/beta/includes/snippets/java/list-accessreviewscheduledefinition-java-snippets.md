---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: b7d69e3f1936d95c53a84240f9c778c73bb8edeb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214180"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewScheduleDefinitionCollectionPage definitions = graphClient.identityGovernance().accessReviews().definitions()
    .buildRequest()
    .skip(0)
    .top(100)
    .get();

```