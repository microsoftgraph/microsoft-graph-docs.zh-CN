---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae477f537ce0cff593cbcbc0ba2c2e4e446e1723aa4d95e02edecdb354a8d758
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104109"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewScheduleDefinition = {
  displayName: 'Review employee access to LinkedIn',
  descriptionForAdmins: 'Review employee access to LinkedIn',
  scope: {
    '@odata.type': '#microsoft.graph.principalResourceMembershipsScope',
    principalScopes: [
      {
        '@odata.type': '#microsoft.graph.accessReviewQueryScope',
        query: '/users',
        queryType: 'MicrosoftGraph'
      }
    ],
    resourceScopes: [
      {
        '@odata.type': '#microsoft.graph.accessReviewQueryScope',
        query: '/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae',
        queryType: 'MicrosoftGraph'
      }
    ]
  },
  reviewers: [
    {
      query: './manager',
      queryType: 'MicrosoftGraph',
      queryRoot: 'decisions'
    }
  ],
  backupReviewers: [
    {
      query: '/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers',
      queryType: 'MicrosoftGraph'
    }
  ],
  fallbackReviewers: [
    {
      query: '/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers',
      queryType: 'MicrosoftGraph'
    }
  ],
  settings: {
    mailNotificationsEnabled: true,
    reminderNotificationsEnabled: true,
    justificationRequiredOnApproval: true,
    defaultDecisionEnabled: true,
    defaultDecision: 'Recommendation',
    instanceDurationInDays: 180,
    autoApplyDecisionsEnabled: true,
    recommendationsEnabled: true,
    recurrence: {
      pattern: {
        type: 'absoluteMonthly',
        interval: 6,
        dayOfMonth: 0
      },
      range: {
        type: 'numbered',
        startDate: '2021-05-05',
        endDate: '2022-05-05'
      }
    }
  }
};

await client.api('/identityGovernance/accessReviews/definitions')
    .version('beta')
    .post(accessReviewScheduleDefinition);

```