---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7e2766cca2c2cff2b9ff2007d5557d525bb3fc31
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .version('beta')
    .get();

```