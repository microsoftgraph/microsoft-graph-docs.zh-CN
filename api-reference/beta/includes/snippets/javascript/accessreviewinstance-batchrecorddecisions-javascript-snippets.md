---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e059b151cec8cc854c3c0c650e0ef0789e333f0b58ba920a47a3cbc90ab23b0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902688"
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