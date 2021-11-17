---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71b91cd3423bac1100e6662cdf23acfaeea1f1c8e4377f865a7487951d225973
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902725"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewDecisionCollectionPage myDecisions = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").myDecisions()
    .buildRequest()
    .get();

```