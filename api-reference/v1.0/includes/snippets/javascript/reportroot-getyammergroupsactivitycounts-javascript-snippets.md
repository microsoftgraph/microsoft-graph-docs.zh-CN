---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 678214ebce17cfb1cbb4d3e218cc4d2fb7f2fe04
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493271"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityCounts(period='D7')')
    .get();

```