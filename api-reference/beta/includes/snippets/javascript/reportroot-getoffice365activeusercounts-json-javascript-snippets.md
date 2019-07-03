---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e3c9b244ecfe46d3ab05a481358e527473fe37c6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActiveUserCounts(period='D7')')
    .version('beta')
    .get();

```