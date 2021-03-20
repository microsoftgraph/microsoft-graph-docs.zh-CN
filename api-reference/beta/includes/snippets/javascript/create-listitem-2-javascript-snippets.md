---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6585d2a605c406c41c7fbaa4fb5bc7f797073cfc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942381"
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