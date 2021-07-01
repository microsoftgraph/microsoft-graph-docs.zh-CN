---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba3a740287dd651653a10563be4b16f66127245c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209726"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItem accessReviewInstanceDecisionItem = graphClient.identityGovernance().accessReviews().definitions("abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd").instances("abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd").decisions("9550e25b-f315-4454-9d87-16b885c35de4")
    .buildRequest()
    .get();

```