---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83b7a0c5d060a23a9a75843c964cd484e1f4d08b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44338984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/oauth2PermissionGrants/{id}')
    .version('beta')
    .get();

```