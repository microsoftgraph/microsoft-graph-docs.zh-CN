---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 948b6bdbf108208806fa39e49c7eb9b729fb2032
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559648"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalAttachment')
    .version('beta')
    .get();

```