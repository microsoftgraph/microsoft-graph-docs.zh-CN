---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89d8fe187e82416056b24a81c86294d90ae4745aa9dd361ce6bd629e164f02ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334011"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdminConsentRequestPolicy adminConsentRequestPolicy = new AdminConsentRequestPolicy();
adminConsentRequestPolicy.isEnabled = true;
adminConsentRequestPolicy.notifyReviewers = true;
adminConsentRequestPolicy.remindersEnabled = true;
adminConsentRequestPolicy.requestDurationInDays = 5;
LinkedList<AccessReviewReviewerScope> reviewersList = new LinkedList<AccessReviewReviewerScope>();
AccessReviewReviewerScope reviewers = new AccessReviewReviewerScope();
reviewers.query = "/users/b6879be8-fb87-4482-a72e-18445d2b5c54";
reviewers.queryType = "MicrosoftGraph";
reviewersList.add(reviewers);
AccessReviewReviewerScope reviewers1 = new AccessReviewReviewerScope();
reviewers1.query = "/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9";
reviewers1.queryType = "MicrosoftGraph";
reviewersList.add(reviewers1);
adminConsentRequestPolicy.reviewers = reviewersList;

graphClient.policies().adminConsentRequestPolicy()
    .buildRequest()
    .put(adminConsentRequestPolicy);

```