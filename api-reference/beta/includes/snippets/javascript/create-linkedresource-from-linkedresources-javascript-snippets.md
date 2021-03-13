---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5179c06fc1b4d507d0b98a5c92776c09ab31d6d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const linkedResource = {
  webUrl: 'https://microsoft.com',
  applicationName: 'Microsoft',
  displayName: 'Microsoft',
  externalId: 'dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9'
};

await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources')
    .version('beta')
    .post(linkedResource);

```