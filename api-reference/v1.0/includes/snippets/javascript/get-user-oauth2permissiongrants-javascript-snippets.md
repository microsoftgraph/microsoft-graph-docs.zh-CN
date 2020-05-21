---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64fb48fd781bf8c4832bc54816877a9d8767e62f
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/oauth2PermissionGrants')
    .get();

```