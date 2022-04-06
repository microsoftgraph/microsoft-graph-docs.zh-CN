---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 589bb3f63e812ee92bf9197112b492e8ef796633
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758096"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drive/items/{bundle-id}')
    .version('beta')
    .delete();

```