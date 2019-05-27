---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7c37218459ae43302ae2b2462031317843d278bb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/children')
    .version('beta')
    .get();

```