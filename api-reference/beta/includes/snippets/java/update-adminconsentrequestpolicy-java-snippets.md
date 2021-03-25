---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fa87c0c2e8dd66db6bacc853a87d7935e88bf55
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201464"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdminConsentRequestPolicy adminConsentRequestPolicy = new AdminConsentRequestPolicy();
adminConsentRequestPolicy.isEnabled = true;
adminConsentRequestPolicy.notifyReviewers = true;
adminConsentRequestPolicy.remindersEnabled = true;
adminConsentRequestPolicy.requestDurationInDays = 5;
LinkedList<AccessReviewScope> reviewersList = new LinkedList<AccessReviewScope>();
AccessReviewScope reviewers = new AccessReviewScope();
reviewers.query = "/users/b6879be8-fb87-4482-a72e-18445d2b5c54";
reviewers.queryType = "MicrosoftGraph";
reviewersList.add(reviewers);
AccessReviewScope reviewers1 = new AccessReviewScope();
reviewers1.query = "/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9";
reviewers1.queryType = "MicrosoftGraph";
reviewersList.add(reviewers1);
adminConsentRequestPolicy.reviewers = reviewersList;

graphClient.policies().adminConsentRequestPolicy()
    .buildRequest()
    .put(adminConsentRequestPolicy);

```