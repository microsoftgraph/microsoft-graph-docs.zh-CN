---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c07343d64a9225a763979b4fa1d4f458cfc33ed7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973251"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItemCollectionPage decisions = graphClient.identityGovernance().accessReviews().definitions("60860cdd-fb4d-4054-91ba-444404f3baa6").instances("14444cdb-6a18-4c08-ba2c-48c02f0a0138").decisions()
    .buildRequest()
    .skip(0)
    .top(100)
    .get();

```