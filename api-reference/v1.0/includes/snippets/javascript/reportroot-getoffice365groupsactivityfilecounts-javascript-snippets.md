---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 758f01a851e287af2a747ad5bf4ab9bb33416513
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityFileCounts(period='D7')')
    .get();

```