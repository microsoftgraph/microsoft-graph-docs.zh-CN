---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5801981b0c56b7a5f74a54327ec2970cd90c771f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208686"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewScheduleDefinitionCollectionPage definitions = graphClient.identityGovernance().accessReviews().definitions()
    .buildRequest()
    .filter("contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')")
    .get();

```