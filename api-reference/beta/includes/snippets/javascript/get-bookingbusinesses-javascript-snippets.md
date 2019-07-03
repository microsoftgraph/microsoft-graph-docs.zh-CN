---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a9b8cae5c796eddb52b507e63199176a2d3845ef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses')
    .version('beta')
    .get();

```