---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 707d18577d323723a5ca81e777a5b9cc496c100a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/oauth2PermissionGrants')
    .get();

```