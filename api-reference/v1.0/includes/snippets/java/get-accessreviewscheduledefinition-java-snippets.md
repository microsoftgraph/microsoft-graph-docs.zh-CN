---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 757bf20f91cbf9d696264cd9f75a951b45883507ca4867e76b66757ae57e1f26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278239"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewScheduleDefinition accessReviewScheduleDefinition = graphClient.identityGovernance().accessReviews().definitions("3856fd6f-36e2-4152-97c9-76070d19f730")
    .buildRequest()
    .get();

```