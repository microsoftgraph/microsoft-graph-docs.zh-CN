---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 123ab684e0340a2894ed2ac0f3840c3a6d4692d215c1ff2f085af7f62cf33f75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902619"
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
    '@odata.type': '#microsoft.graph.accessReviewQueryScope',
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