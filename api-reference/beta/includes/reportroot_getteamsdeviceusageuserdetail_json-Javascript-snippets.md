---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a9863db4e3c60bd7aaa90679e2bae7ebe6bc05ab
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481735"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsDeviceUsageUserDetail(period='D7')')
    .version('beta')
    .get();

```