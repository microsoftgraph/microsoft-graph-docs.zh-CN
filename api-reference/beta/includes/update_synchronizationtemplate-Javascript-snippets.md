---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 20759b72063bba3aa76f15d03e5a35ac10b5e41f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475946"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationTemplate = {
    id: "Slack",
    applicationId: "{id}",
    factoryTag: "CustomSCIM"
};

let res = await client.api('/applications/{id}/synchronization/templates/{templateId}')
    .version('beta')
    .put({synchronizationTemplate : synchronizationTemplate});

```