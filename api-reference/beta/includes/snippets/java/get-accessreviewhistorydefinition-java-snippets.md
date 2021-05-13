---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b070d09579204ad0f663e0a9745873ab5f0a05c
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474178"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewHistoryDefinition accessReviewHistoryDefinition = graphClient.identityGovernance().accessReviews().historyDefinitions("b2cb022f-b7e1-40f3-9854-c65a40861c38")
    .buildRequest()
    .get();

```