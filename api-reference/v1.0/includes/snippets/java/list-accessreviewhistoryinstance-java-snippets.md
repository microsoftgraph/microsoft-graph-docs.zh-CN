---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08fd9a8e5a98023fe75206df6279604d80f08ea1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337638"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewHistoryInstanceCollectionPage instances = graphClient.identityGovernance().accessReviews().historyDefinitions("90e28cb7-4b9a-48f7-ba4e-a2756fda01b2").instances()
    .buildRequest()
    .get();

```