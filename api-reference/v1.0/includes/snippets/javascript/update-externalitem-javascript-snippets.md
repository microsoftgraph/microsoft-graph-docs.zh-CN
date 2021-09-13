---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e92d4c1fb88ad825339c7110f71b4937848c017c5e33de9efc8a3268298641ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  acl: [
    {
      type: 'everyone',
      value: '67a141d8-cf4e-4528-ba07-bed21bfacd2d',
      accessType: 'grant'
    }
  ]
};

await client.api('/connections/contosohr/items/TSP228082938')
    .update(externalItem);

```