---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5244ae5193c1717f9798b86f548ef109661c402d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityGroupCounts(period='D7')')
    .version('beta')
    .get();

```