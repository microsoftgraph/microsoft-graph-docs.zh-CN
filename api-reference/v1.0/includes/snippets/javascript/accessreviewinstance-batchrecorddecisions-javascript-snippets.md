---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 264fc464ab02ece037bb6b2d7afb34c4b3edf253c8212adb0f7ec00b490dd1a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331852"
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

await client.api('/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-6778-8868-9999c7f4cc06/batchRecordDecisions')
    .post(batchRecordDecisions);

```