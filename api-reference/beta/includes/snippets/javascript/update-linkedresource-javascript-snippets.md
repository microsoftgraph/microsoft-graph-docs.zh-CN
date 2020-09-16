---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1137cde7487f5ed3a41d6027b35d93fc5a988b13
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47842937"
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
  displayName: "Microsoft",
};

let res = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9')
    .version('beta')
    .update(linkedResource);

```