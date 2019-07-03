---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 87970838fe8c64d852b0a134389b3d82e894b3d2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityDetail(period='D7')')
    .version('beta')
    .get();

```