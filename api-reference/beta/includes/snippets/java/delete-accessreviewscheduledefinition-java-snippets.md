---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: e3b424ed1235c04143ce52341fb1cc82d72db068
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214247"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("29f2d16e-9ca6-4052-bbfe-802c48981fd8")
    .buildRequest()
    .delete();

```