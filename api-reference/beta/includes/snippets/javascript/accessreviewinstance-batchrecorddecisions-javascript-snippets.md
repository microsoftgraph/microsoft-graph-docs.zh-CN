---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a319a7aed83e33cefb3fa57c91db11c9013105f8
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507475"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const batchRecordDecisions = {
  decision: 'Approve',
  justification: 'All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team',
  resourceId: 'a5c51e59-3fcd-4a37-87a1-835c0c21488a'
};

await client.api('/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions')
    .version('beta')
    .post(batchRecordDecisions);

```