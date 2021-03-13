---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ff1ca58b53505d9848e4beb58dee70176fb8ed7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewScheduleDefinition = {
  displayName: 'Test create',
  descriptionForAdmins: 'New scheduled access review',
  descriptionForReviewers: 'If you have any questions, contact jerry@contoso.com',
  scope: {
    query: '/groups/b7a059cb-038a-4802-8fc9-b9d1ed0c4444/transitiveMembers',
    queryType: 'MicrosoftGraph'
  },
  reviewers: [
    {
      query: '/users/7eae4444-d425-48b2-adf2-3c777f6256f3',
      queryType: 'MicrosoftGraph',
      queryRoot: 'decisions'
    }
  ],
  settings: {
    mailNotificationsEnabled: true,
    reminderNotificationsEnabled: true,
    justificationRequiredOnApproval: true,
    defaultDecisionEnabled: false,
    defaultDecision: 'None',
    instanceDurationInDays: 1,
    autoApplyDecisionsEnabled: false,
    recommendationsEnabled: true,
    recurrence: {
      pattern: {
        type: 'weekly',
        interval: 1
      },
      range: {
        type: 'noEnd',
        startDate: '2020-09-08T12:02:30.667Z'
      }
    }
  }
};

await client.api('/identityGovernance/accessReviews/definitions')
    .version('beta')
    .post(accessReviewScheduleDefinition);

```