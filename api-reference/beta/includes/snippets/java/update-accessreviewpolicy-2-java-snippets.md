---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef3888c4306f6a935722cf40896f27406e5f2f64
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240622"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewPolicy accessReviewPolicy = new AccessReviewPolicy();
accessReviewPolicy.isGroupOwnerManagementEnabled = true;

graphClient.identityGovernance().accessReviews().policy()
    .buildRequest()
    .patch(accessReviewPolicy);

```