---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b64b206a9659599c0da129e3f6c2e0d99c30c06
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335637"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/appRoleAssignments')
    .version('beta')
    .get();

```