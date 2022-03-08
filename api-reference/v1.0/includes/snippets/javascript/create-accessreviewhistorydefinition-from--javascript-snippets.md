---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25658262a5c8c95a43aedbed4639f6d70e9e852c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewHistoryDefinition = {
  displayName: 'Last quarter\'s group reviews April 2021',
  decisions: [
    'approve',
    'deny',
    'dontKnow',
    'notReviewed',
    'notNotified'
  ],
  scheduleSettings: {
      reportRange: 'P1M',
      recurrence: {
          pattern: {
              type: 'monthly',
              interval: 1
          },
          range: {
              type: 'noEnd',
              startDate: '2018-08-03T21:02:30.667Z',
              count: 0
          }
        }
  },
  scopes: [
    {
      '@odata.type': '#microsoft.graph.accessReviewQueryScope',
      queryType: 'MicrosoftGraph',     
      query: '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'accessPackageAssignments\')',
      queryRoot: null
    },  
    {
      '@odata.type': '#microsoft.graph.accessReviewQueryScope',
      queryType: 'MicrosoftGraph',     
      query: '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'/groups\')',
      queryRoot: null
    }
  ]
};

await client.api('/identityGovernance/accessReviews/historyDefinitions')
    .post(accessReviewHistoryDefinition);

```