---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 077f7fe662852be683faebccb4f1de0889ce06d8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/administrativeUnits/{id}')
    .version('beta')
    .get();

```