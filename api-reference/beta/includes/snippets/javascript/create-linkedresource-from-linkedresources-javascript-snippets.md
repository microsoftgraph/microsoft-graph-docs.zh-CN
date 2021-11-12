---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0ba01d1a336cbf9493b453c4f5254462e1cc15e0286c8c0416348b48fb1b742
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333690"
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