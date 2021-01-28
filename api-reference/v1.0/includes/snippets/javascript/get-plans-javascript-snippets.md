---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d5213a93c4e287fae1bec1263f051a222d1aafd
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans')
    .get();

```