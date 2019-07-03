---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e5e5057e8a0381c3b1a45c5dbed20e5020ddbbd4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/profileStatus')
    .version('beta')
    .get();

```