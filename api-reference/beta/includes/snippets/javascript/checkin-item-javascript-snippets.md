---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecdc5a15a1178bcfe32c5a09d43cd05c09480ec4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const checkin = {
  comment: "Updating the latest guidelines"
};

let res = await client.api('/drives/{drive-id}/items/{item-id}/checkin')
    .version('beta')
    .post(checkin);

```