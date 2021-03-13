---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f179889937cf29e4d14eb6dd02d3b8c8375c873
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805762"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/planner/all/delta')
    .version('beta')
    .get();

```