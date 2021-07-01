---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe23039abd55e2d826c2da9f9ea68afc93597866
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209796"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItemCollectionPage decisions = graphClient.identityGovernance().accessReviews().definitions("abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd").instances("7070ea1c-8d12-457b-bd35-a37dc59e54e0").decisions()
    .buildRequest()
    .get();

```