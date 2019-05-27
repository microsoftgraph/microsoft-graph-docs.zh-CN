---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ecd9f7d4eea14e437274c69808ea975946e7c92d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com/verify')
    .version('beta')
    .post();

```