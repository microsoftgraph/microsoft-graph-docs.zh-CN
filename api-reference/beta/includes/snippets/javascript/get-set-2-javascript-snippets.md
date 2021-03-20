---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 488bb0f9d7bda5bd2d49cc979ae385a58615b493
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955404"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let set = await client.api('/termStore/sets/{setId}')
    .version('beta')
    .get();

```