---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8dfa0be5e8ddbe891c98fe8b80a3816caf6bd9df
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436990"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/subscriptions/socketIo')
    .version('beta')
    .get();

```