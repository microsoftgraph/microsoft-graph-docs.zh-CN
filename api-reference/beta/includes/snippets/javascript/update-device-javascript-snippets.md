---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a3b30c8316991cc877a1f4d061571f85f481fbe0
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: false
};

let res = await client.api('/devices/{id}')
    .version('beta')
    .update(device);

```