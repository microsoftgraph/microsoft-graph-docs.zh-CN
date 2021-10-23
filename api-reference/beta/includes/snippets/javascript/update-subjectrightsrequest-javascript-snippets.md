---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec348164cccddf8480f2940e2a549e2dff1cd3ae
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559602"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subjectRightsRequest = {
  '@odata.type': '#microsoft.graph.subjectRightsRequest',
  internalDueDateTime: '2021-08-30T00:00:00Z'
};

await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}')
    .version('beta')
    .update(subjectRightsRequest);

```