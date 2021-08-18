---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0af8b1e4b66288ff4a9202c05c2953633f5751c093766ce471f7a0926da52fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewScheduleDefinition = {
  id: '60860cdd-fb4d-4054-91ba-f75e04444aa6',
  displayName: 'Test world UPDATED NAME!',
  descriptionForAdmins: 'Test world',
  descriptionForReviewers: 'Test world',
  scope: {
    query: '/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers',
    queryType: 'MicrosoftGraph'
  },
  instanceEnumerationScope: {
    query: '/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f',
    queryType: 'MicrosoftGraph'
  },
  reviewers: [],
  settings: {
    mailNotificationsEnabled: true,
    reminderNotificationsEnabled: true,
    justificationRequiredOnApproval: true,
    defaultDecisionEnabled: false,
    defaultDecision: 'None',
    instanceDurationInDays: 3,
    autoApplyDecisionsEnabled: false,
    recommendationsEnabled: true,
    recurrence: {
      pattern: {
        type: 'weekly',
        interval: 1
      },
      range: {
        type: 'noEnd',
        startDate: '2020-09-15'
      }
    }
  }
};

await client.api('/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6')
    .put(accessReviewScheduleDefinition);

```