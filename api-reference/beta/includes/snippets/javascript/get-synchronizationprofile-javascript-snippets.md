---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0a8ac90e5f534082931e2e4c1799c288c6953b30
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500119"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}')
    .version('beta')
    .delete();

```