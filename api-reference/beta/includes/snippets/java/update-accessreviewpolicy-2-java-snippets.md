---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9aa2d1dbfa7a0c6e20f4424ddcf4059c028c30d265746c48dbd73861b2c2201b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104121"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewPolicy accessReviewPolicy = new AccessReviewPolicy();
accessReviewPolicy.isGroupOwnerManagementEnabled = true;

graphClient.identityGovernance().accessReviews().policy()
    .buildRequest()
    .patch(accessReviewPolicy);

```