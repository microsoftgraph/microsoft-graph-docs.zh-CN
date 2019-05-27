---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b1e2d9655e2fb2808d176a9a6109c303214a71f0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447173"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programControls')
    .version('beta')
    .get();

```