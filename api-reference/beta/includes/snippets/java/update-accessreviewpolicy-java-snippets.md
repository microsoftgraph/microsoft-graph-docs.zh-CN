---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d537f737d37ccf89841d2238839ce90fc91b65f
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240641"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewPolicy accessReviewPolicy = new AccessReviewPolicy();
accessReviewPolicy.isGroupOwnerManagementEnabled = true;

graphClient.policies().accessReviewPolicy()
    .buildRequest()
    .patch(accessReviewPolicy);

```