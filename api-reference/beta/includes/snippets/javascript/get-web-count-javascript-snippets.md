---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b669c88b815f8d2ae4403e149bba42434d9ce604
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applications = await client.api('/applications')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Web')
    .get();

```