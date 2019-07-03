---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8fd66bd2e493bb3ef6febb74a556e2f6a1fdd964
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```