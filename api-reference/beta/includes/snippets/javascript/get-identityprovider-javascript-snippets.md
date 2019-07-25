---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c83a03e1c4b8e1fadd5ff34add7e5edcba11f5b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders/Amazon-OAuth')
    .version('beta')
    .get();

```