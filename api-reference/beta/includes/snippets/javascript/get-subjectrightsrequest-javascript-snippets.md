---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69883c6034c683e62a9d754b0c81838e41c46a02
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subjectRightsRequest = await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}')
    .version('beta')
    .get();

```