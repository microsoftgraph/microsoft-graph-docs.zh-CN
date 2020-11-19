---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 56531f5a27cc1ec0dd40f7266d347a05704837f3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214759"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("04e5c3b2-9db2-40d3-a204-128f4956ae8e").instances("70463350-742e-4909-bfa5-bc23447bd002")
    .applyDecisions()
    .buildRequest()
    .post();

```