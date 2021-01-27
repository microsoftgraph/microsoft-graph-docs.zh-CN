---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f88b1723a778c1e828f48f2bdb3528484fba8370
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015764"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/10001/users/13006')
    .version('beta')
    .delete();

```