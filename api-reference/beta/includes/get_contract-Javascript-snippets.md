---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e9e12670caaa15b33d78ce1294e7b48a2ce64fb1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472523"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contracts')
    .version('beta')
    .get();

```