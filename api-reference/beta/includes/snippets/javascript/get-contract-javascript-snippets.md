---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 293824a8bf73f6907a8068b200ebb557c3217ed4
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contracts/{id}')
    .version('beta')
    .get();

```