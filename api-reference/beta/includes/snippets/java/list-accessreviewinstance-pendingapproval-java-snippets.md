---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 30e51c526ada7c5b213bbb4ab74c42fc0f47aebc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222038"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewInstanceCollectionPage pendingAccessReviewInstances = graphClient.me().pendingAccessReviewInstances()
    .buildRequest()
    .expand("definition")
    .skip(0)
    .top(100)
    .get();

```