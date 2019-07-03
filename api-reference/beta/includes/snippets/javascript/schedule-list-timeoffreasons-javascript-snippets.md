---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7e2766cca2c2cff2b9ff2007d5557d525bb3fc31
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499541"
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