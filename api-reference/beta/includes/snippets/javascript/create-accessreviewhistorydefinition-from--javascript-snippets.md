---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecde4d23820a9ccd37be6aa038c82b889d391472
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352560"
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
    .version('beta')
    .post(accessReviewHistoryDefinition);

```