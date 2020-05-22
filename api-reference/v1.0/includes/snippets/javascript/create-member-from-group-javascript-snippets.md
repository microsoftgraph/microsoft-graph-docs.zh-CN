---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe67ee072d03d1808c511dbab7eba00e97befb6c
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44338901"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  members@odata.bind: [
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
    ]
};

let res = await client.api('/groups/{id}')
    .update(group);

```