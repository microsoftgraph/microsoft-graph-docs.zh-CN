---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf18f03547c4bd9add213079e84b2da9c77ab7ec0485a1da766ef36f1e8d8464
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105024"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceCollectionPage instances = graphClient.identityGovernance().accessReviews().definitions("2dca8959-b716-4b4c-a93d-a535c01eb6e0").instances()
    .buildRequest()
    .get();

```