---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3b59ddd3779d1d1ad10e67d174ad41e4ab74ad75
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636597"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
    displayName: "Seattle District Technical Schools",
    description: "Seattle district technical schools administration",
    visibility: "true"
};

let res = await client.api('/administrativeUnits')
    .version('beta')
    .post(administrativeUnit);

```