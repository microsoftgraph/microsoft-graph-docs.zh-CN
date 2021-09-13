---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0eff8f3f1247f68c1059d2d86d9061a5177738ac4849c3ba59f34184bb027b72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902520"
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
    .post(linkedResource);

```