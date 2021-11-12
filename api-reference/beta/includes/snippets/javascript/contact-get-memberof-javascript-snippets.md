---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a7108af33ebc9c3c3a336574d1e4a3163f2ec28fcaea208168d00cbe6142a38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .get();

```