---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55c7612e425aeb9bc208e6c5ab7775df9d62a93c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092932"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/cases/eDiscoveryCases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen')
    .version('beta')
    .post();

```