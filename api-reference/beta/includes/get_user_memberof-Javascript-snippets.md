---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3dfa5d99c2a3e48237dddafa3f7b563c95109d80
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445180"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/memberOf')
    .version('beta')
    .get();

```