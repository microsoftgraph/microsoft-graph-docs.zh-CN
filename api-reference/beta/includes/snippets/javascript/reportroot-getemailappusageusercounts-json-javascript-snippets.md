---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 00c1580c9d377bc2ceef004f8e4dfea47bce94f3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageUserCounts(period='D7')')
    .version('beta')
    .get();

```