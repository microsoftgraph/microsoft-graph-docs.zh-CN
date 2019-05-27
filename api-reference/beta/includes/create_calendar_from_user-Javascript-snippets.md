---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0363adf0e351f521aed0e0e447d91cc2826e1b2c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434404"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Volunteer"
};

let res = await client.api('/me/calendars')
    .version('beta')
    .post({calendar : calendar});

```