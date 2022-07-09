---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95ab65fdcf3d90ab7150c96be0742243f738c5a1
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854038"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewStage = {
  '@odata.type': '#microsoft.graph.accessReviewStage',
  reviewers: [
      {
          query: '/users/1ed8ac56-4827-4733-8f80-86adc2e67db5',
          queryType: 'MicrosoftGraph'
      }
  ],
  fallbackReviewers: [
      {
          query: '/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e',
          queryType: 'MicrosoftGraph'
      },
      {
          query: '/users/1ed8ac56-4827-4733-8f80-86adc2e67db5',
          queryType: 'MicrosoftGraph'
      }
  ]
};

await client.api('/identityGovernance/accessReviews/definitions/5dcfcc88-da88-4252-8629-a0807b4b076d/instances/720b8ee0-cee4-42ac-b164-894c48703acc/stages/7d244ab1-4ab1-7d24-b14a-247db14a247d')
    .version('beta')
    .update(accessReviewStage);

```