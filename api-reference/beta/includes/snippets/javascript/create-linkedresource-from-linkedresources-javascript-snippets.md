---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9df22a6ac2a23a9f466390a3e992407eeb96ada8
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const linkedResource = {
  @odata.type: "#microsoft.graph.linkedResource",
  webUrl: "http:://microsoft.com",
  applicationName: "Microsoft",
  displayName: "Microsoft",
  externalId: "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
};

let res = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources')
    .version('beta')
    .post(linkedResource);

```