---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a7214b189d04f26e5797d0662111b825a73a16d
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/delta')
    .version('beta')
    .get();

```