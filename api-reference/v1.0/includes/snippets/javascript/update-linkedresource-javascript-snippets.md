---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 442198bbc58e141149452c06a4eda4de96b95fb5
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903402"
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
    .update(linkedResource);

```