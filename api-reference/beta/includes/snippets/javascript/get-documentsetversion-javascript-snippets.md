---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6fd9d0b33ddf358b80051db88c87713e1a6e0cb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210285"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let documentSetVersion = await client.api('/sites/root/lists/Documents/items/2/documentSetVersions/1')
    .version('beta')
    .get();

```