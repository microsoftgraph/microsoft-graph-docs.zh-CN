---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb57af98a5fa33e2b483c37cd3e7be1a3d64c4907b90b481c87e2127d18d1cf3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const fieldValueSet = {
    Color: 'Fuchsia',
    Quantity: 934
};

await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/fields')
    .version('beta')
    .update(fieldValueSet);

```