---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1311cca94134e812eb49288eb19506d5b1314abbba5562c7ca09022093d1c352
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104127"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItemCollectionPage decisions = graphClient.me().pendingAccessReviewInstances("70a68410-67f3-4d4c-b946-6989e050be19").decisions()
    .buildRequest()
    .skip(0)
    .top(100)
    .get();

```