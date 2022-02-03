---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08fd9a8e5a98023fe75206df6279604d80f08ea1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340557"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewHistoryInstanceCollectionPage instances = graphClient.identityGovernance().accessReviews().historyDefinitions("90e28cb7-4b9a-48f7-ba4e-a2756fda01b2").instances()
    .buildRequest()
    .get();

```