---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9086dc22f63e02d31109fde29900693c8ed47d80
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityCounts(period='D7')')
    .version('beta')
    .get();

```