---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ced8e164b46b1d9d4a1ddf4e0891680c5fe25c1e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664585"
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
    query: '/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers',
    queryType: 'MicrosoftGraph'
  },
  reviewers: [
    {
      query: '/users/398164b1-5196-49dd-ada2-364b49f99b27',
      queryType: 'MicrosoftGraph'
    }
  ],
  settings: {
    mailNotificationsEnabled: true,
    reminderNotificationsEnabled: true,
    justificationRequiredOnApproval: true,
    defaultDecisionEnabled: false,
    defaultDecision: 'None',
    instanceDurationInDays: 1,
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