---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 87bdee94f609ce40dc4ae2189a835ff9303d3dcf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439426"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationTemplate = {
    id: "SCIM-Test1",
    applicationId: "{id}",
    factoryTag: "CustomSCIM"
};

let res = await client.api('/applications/{id}/synchronization/templates')
    .version('beta')
    .post({synchronizationTemplate : synchronizationTemplate});

```