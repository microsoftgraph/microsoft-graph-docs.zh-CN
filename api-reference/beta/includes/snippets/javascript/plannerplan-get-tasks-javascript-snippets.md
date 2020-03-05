---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6f0ff6063c5ad9ef31a50816ad56f21ab58acc0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/tasks')
    .version('beta')
    .get();

```