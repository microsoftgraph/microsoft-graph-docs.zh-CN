---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5115e7dfa9061d9927a31d147912c96bb3a24300
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const linkedResource = {
  webUrl: "https://microsoft.com",
  applicationName: "Microsoft",
  displayName: "Microsoft",
  externalId: "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
};

let res = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources')
    .post(linkedResource);

```