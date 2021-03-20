---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf038a1287b61df4276ec9b04e3b29a34589d60b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicies = await client.api('/groupLifecyclePolicies')
    .version('beta')
    .get();

```