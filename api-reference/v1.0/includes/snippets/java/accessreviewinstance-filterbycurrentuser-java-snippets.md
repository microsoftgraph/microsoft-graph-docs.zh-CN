---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d5587dabb5503030eab7ce6ef98d564502dcbc758b1fd69757c18bfd4152960
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278630"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().accessReviews().definitions("e6cafba0-cbf0-4748-8868-0810c7f4cc06").instances()
    .filterByCurrentUser(AccessReviewInstanceFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('reviewer')
        .build())
    .buildRequest()
    .get();

```