---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be0b8c98f0e5fef99644c5665cd0007fb3df2e26
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let submissions = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/efcdf80b-a5de-42ac-8579-e40b0223d48b/submissions')
    .version('beta')
    .expand('outcomes')
    .get();

```