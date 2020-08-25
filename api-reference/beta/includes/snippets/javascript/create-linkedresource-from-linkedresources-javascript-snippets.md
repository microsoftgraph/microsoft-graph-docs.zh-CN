---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c1568a9fa7c71266bcd7c815986239f6a7845de
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873244"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const linkedResources = {
  @odata.type: "#microsoft.graph.linkedResource",
  webUrl: "http:://microsoft.com",
  applicationName: "Microsoft",
  displayName: "Microsoft",
  externalId: "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
};

let res = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources')
    .version('beta')
    .post(linkedResources);

```