---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f54a5e65f25ba633c262c96d64e3ef701b6e7288c24288974efba8f3477b812d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902730"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewCollectionPage accessReviews = graphClient.accessReviews()
    .buildRequest()
    .filter("businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68'")
    .skip(0)
    .top(100)
    .get();

```