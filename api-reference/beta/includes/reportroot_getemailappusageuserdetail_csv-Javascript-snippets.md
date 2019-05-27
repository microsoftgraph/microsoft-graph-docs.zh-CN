---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9f8547294388b0d3d8ff141e1da2fc6cf9a9d2c2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageUserDetail(period='D7')')
    .version('beta')
    .get();

```