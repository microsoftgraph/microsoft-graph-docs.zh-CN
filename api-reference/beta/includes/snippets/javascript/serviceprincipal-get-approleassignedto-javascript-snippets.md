---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa0949245017647bba941fc378ee2d4dc2a310dd
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/appRoleAssignedTo')
    .version('beta')
    .get();

```