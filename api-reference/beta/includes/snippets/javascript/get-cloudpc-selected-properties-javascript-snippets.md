---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae3db7a2bacf10585517affc5650e9bbfb1b8ffc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPC = await client.api('/deviceManagement/virtualEndpoint/cloudPCs/40cee9d2-03fb-4066-8d35-dbdf2875c33f')
    .version('beta')
    .select('id,displayName,imageDisplayName,lastModifiedDateTime,lastRemoteActionResult,lastLoginResult')
    .get();

```