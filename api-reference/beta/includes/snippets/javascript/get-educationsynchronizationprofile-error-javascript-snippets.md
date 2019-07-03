---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9345fd73eb0d2f8a89876986544c4db22b5eae3c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521466"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/errors')
    .version('beta')
    .get();

```