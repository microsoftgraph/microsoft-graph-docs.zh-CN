---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 96ea3489b37264c11ad76837bb7ecf8dcc8dff66
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessActivityCounts(period='D7')')
    .version('beta')
    .get();

```