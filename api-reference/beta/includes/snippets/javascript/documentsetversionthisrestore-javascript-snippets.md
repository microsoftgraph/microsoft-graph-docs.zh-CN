---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2daae3071065b57209fd7df8e8128e3bf1f40727
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205991"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/root/lists/Documents/items/2/documentSetVersions/1/restore')
    .version('beta')
    .post();

```