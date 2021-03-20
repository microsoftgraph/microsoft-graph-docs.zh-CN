---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4970cc96e33fc0bb5cc8e7c8f829cfd2e3fd13e7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972997"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceCollectionPage instances = graphClient.identityGovernance().accessReviews().definitions("60860cdd-fb4d-4054-91ba-f75e04f34444").instances()
    .buildRequest()
    .skip(0)
    .top(100)
    .get();

```