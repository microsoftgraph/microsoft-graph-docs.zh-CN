---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5a35f480a88639511473d39074a24adb7a7dc7c9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521609"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityFileCounts(period='D7')')
    .version('beta')
    .get();

```