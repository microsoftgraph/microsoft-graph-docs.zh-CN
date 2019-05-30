---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9eeeff72289312701e8fa37764583a1a0df908f2
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536363"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields')
    .version('beta')
    .get();

```