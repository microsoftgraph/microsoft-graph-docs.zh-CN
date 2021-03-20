---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07857ecac9c6c64a0728859fdf3e88ebe31faacc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/servicePrincipals/{id}/synchronization/jobs/')
    .version('beta')
    .get();

```