---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0c48a2ea5644fb5d8f04e1f79ebea03204e62b8d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsUserActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```