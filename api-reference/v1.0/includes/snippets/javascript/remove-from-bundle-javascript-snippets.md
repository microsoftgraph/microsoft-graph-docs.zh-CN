---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d27f885ac8f9fc13075490c667776a87a8a6022
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758224"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drive/bundles/{bundle-id}/children/{item-id}')
    .version('beta')
    .delete();

```