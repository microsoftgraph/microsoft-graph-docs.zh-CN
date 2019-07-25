---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e3c9b244ecfe46d3ab05a481358e527473fe37c6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719090"
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