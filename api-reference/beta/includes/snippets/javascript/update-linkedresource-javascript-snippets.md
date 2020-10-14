---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5b4c91c4af3fd4c5e82659fc772973c5d8c2b6a
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462572"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const linkedResource = {
  @odata.type: "#microsoft.graph.linkedResource",
  webUrl: "http://microsoft.com",
  applicationName: "Microsoft",
  displayName: "Microsoft"
};

let res = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9')
    .version('beta')
    .update(linkedResource);

```