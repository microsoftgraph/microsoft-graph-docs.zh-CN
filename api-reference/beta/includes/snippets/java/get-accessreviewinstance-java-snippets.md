---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: ab94a507f7234fa732eddc65609eb777f8dde2aa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222134"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstance accessReviewInstance = graphClient.identityGovernance().accessReviews().definitions("60860cdd-fb4d-4054-91ba-444404f3baa6").instances("12490cdb-6a18-4c08-ba2c-44442f0a0138")
    .buildRequest()
    .get();

```