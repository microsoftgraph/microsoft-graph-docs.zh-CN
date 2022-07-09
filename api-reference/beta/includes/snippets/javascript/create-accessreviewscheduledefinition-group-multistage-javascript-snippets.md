---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c4f931b0f8e5f399f5f2a2f3312e764d385a84b
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewScheduleDefinition = {
  displayName: 'Group Multi-stage Access Review',
  descriptionForAdmins: 'New scheduled access review',
  descriptionForReviewers: 'If you have any questions, contact jerry@contoso.com',
  scope: {
    '@odata.type': '#microsoft.graph.accessReviewQueryScope',
    query: '/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers',
    queryType: 'MicrosoftGraph'
  },
  stageSettings: [
    {
      stageId: '1',
      durationInDays: 2,
      recommendationsEnabled: false,
      decisionsThatWillMoveToNextStage: [
          'NotReviewed',
          'Approve'
      ],
      reviewers: [
        {
          query: '/users/398164b1-5196-49dd-ada2-364b49f99b27',
          queryType: 'MicrosoftGraph'
        }
      ]
    },
    {
      stageId: '2',
      dependsOn: [
          '1'
      ],
      durationInDays: 2,
      recommendationsEnabled: true,
      reviewers: [
        {
          query: './manager',
          queryType: 'MicrosoftGraph',
          queryRoot: 'decisions'
        }
      ],
      fallbackReviewers: [
        {
          query: '/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers',
          queryType: 'MicrosoftGraph'
        }
      ]
    }
  ],
  settings: {
    mailNotificationsEnabled: true,
    reminderNotificationsEnabled: true,
    justificationRequiredOnApproval: true,
    defaultDecisionEnabled: false,
    defaultDecision: 'None',
    instanceDurationInDays: 4,
    recurrence: {
      pattern: {
        type: 'weekly',
        interval: 1
      },
      range: {
        type: 'noEnd',
        startDate: '2020-09-08T12:02:30.667Z'
      }
    },
    decisionHistoriesForReviewersEnabled: true
  }
};

await client.api('/identityGovernance/accessReviews/definitions')
    .version('beta')
    .post(accessReviewScheduleDefinition);

```