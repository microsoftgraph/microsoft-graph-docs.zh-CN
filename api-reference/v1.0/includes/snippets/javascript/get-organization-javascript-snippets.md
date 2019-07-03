---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 26cfd7e7bc104a6fbbccc9994b29e8d70956c6d0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35468007"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization')
    .version('beta')
    .get();

```