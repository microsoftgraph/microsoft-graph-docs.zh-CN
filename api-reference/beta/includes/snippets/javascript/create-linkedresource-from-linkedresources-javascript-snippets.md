---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94c62909b81867af94465f76cd7c904a077d8489
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48375688"
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
    .version('beta')
    .post(linkedResource);

```