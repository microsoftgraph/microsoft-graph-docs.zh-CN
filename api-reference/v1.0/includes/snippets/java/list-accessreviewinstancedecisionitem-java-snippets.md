---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e34edf23dcd81fb429f4d21d0f396d80dbc0c5e
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53335437"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItemCollectionPage decisions = graphClient.identityGovernance().accessReviews().definitions("2dca8959-b716-4b4c-a93d-a535c01eb6e0").instances("8d035c9d-798d-47fa-beb4-f986a4b8126f").decisions()
    .buildRequest()
    .get();

```