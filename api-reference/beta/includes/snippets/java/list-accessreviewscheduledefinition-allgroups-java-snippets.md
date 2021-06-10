---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5801981b0c56b7a5f74a54327ec2970cd90c771f
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870050"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewScheduleDefinitionCollectionPage definitions = graphClient.identityGovernance().accessReviews().definitions()
    .buildRequest()
    .filter("contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')")
    .get();

```