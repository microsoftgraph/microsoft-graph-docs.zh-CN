---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3859323e6873520fbd379a5058276161b642db77f1737a2b1751f1b6e4acb981
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104153"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewHistoryDefinition accessReviewHistoryDefinition = graphClient.identityGovernance().accessReviews().historyDefinitions("b2cb022f-b7e1-40f3-9854-c65a40861c38")
    .buildRequest()
    .get();

```