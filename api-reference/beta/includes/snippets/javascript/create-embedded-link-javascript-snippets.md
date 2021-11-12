---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51aea3f22dd1c2b571fea4ca2be205f67125623a1eceaee401a0e012a8136aa5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: 'embed'
};

await client.api('/me/drive/items/{item-id}/createLink')
    .version('beta')
    .post(permission);

```