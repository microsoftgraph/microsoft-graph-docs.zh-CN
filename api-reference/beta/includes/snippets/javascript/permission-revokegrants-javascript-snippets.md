---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1800d79d23ad12184f02b87cb6b304f855f0d030
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635467"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = Content-Type: application/json
Content-length: 95

{
  grantees: [
    {
      email: "ryan@contoso.com"
    }
  ]
};

let res = await client.api('/me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants')
    .version('beta')
    .post(permission);

```