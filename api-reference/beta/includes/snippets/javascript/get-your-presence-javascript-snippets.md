---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18b8b2840d027eb0a1e7c2494b452d18a47b9d01938c6cb0964123d5fcd919d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let presence = await client.api('/me/presence')
    .version('beta')
    .get();

```