---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 753f72d2ff458eeb8795e9d3ce361267636594f3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521151"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/settings')
    .version('beta')
    .get();

```