---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 9b8f07476ca106e481427ec3a2b13c4c96cbc5d6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221992"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("2b83cc42-09db-46f6-8c6e-16fec466a82d").instances("61a617dd-238f-4037-8fa5-d800e515f5bc")
    .stop()
    .buildRequest()
    .post();

```