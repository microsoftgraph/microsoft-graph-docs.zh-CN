---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce6da6532711f7164f3b5fa701deca93ff6db604748a3e66ac5e093ffec019f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drives/{drive-id}/items/{item-id}/checkout')
    .version('beta')
    .post();

```