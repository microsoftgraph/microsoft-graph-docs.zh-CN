---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3ab855c9a5b3cba1877953e568e7282d51c13a9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440515"
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
    .post(accessReviewScheduleDefinition);

```