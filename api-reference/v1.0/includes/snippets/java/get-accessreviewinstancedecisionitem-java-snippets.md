---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2ede9b6e5a021753aec803c4b04ea38f8002e82ecb84abe80ce62a5f5c0c512
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409387"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItem accessReviewInstanceDecisionItem = graphClient.identityGovernance().accessReviews().definitions("abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd").instances("abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd").decisions("9550e25b-f315-4454-9d87-16b885c35de4")
    .buildRequest()
    .get();

```