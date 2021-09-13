---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b597803475e6e5a2c7274c459ade4a41bb3128c54c58905fb22f0ae727bbe5fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161607"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: [ 'read' ]
};

await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .update(permission);

```