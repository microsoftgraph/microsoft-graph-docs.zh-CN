---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 680ec5a397f3f8167b2339293be0c35773e2980d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207436"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItem accessReviewInstanceDecisionItem = graphClient.identityGovernance().accessReviews().definitions("5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0").instances("6444d4fd-ab55-4608-8cf9-c6702d172bcc").decisions("e6cafba0-cbf0-4748-8868-0810c7f4cc06")
    .buildRequest()
    .get();

```