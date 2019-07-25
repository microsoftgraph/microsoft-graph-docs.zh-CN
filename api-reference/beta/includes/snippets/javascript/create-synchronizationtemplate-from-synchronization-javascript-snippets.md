---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 87bdee94f609ce40dc4ae2189a835ff9303d3dcf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717295"
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