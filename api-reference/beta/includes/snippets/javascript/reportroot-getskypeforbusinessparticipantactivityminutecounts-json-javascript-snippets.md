---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4f77c0a973fe142738a8914caa1dff950208bec5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')')
    .version('beta')
    .get();

```