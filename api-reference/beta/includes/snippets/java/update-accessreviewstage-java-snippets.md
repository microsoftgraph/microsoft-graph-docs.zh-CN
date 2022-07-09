---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 929c1e742188a165af472e32926ae7968512cfd0
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854044"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewStage accessReviewStage = new AccessReviewStage();
LinkedList<AccessReviewReviewerScope> reviewersList = new LinkedList<AccessReviewReviewerScope>();
AccessReviewReviewerScope reviewers = new AccessReviewReviewerScope();
reviewers.query = "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5";
reviewers.queryType = "MicrosoftGraph";
reviewersList.add(reviewers);
accessReviewStage.reviewers = reviewersList;
LinkedList<AccessReviewReviewerScope> fallbackReviewersList = new LinkedList<AccessReviewReviewerScope>();
AccessReviewReviewerScope fallbackReviewers = new AccessReviewReviewerScope();
fallbackReviewers.query = "/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e";
fallbackReviewers.queryType = "MicrosoftGraph";
fallbackReviewersList.add(fallbackReviewers);
AccessReviewReviewerScope fallbackReviewers1 = new AccessReviewReviewerScope();
fallbackReviewers1.query = "/users/1ed8ac56-4827-4733-8f80-86adc2e67db5";
fallbackReviewers1.queryType = "MicrosoftGraph";
fallbackReviewersList.add(fallbackReviewers1);
accessReviewStage.fallbackReviewers = fallbackReviewersList;

graphClient.identityGovernance().accessReviews().definitions("5dcfcc88-da88-4252-8629-a0807b4b076d").instances("720b8ee0-cee4-42ac-b164-894c48703acc").stages("7d244ab1-4ab1-7d24-b14a-247db14a247d")
    .buildRequest()
    .patch(accessReviewStage);

```