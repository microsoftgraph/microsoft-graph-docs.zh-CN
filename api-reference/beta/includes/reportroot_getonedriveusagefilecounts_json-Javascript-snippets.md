---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2f89bbb2984203b197f4adc835dd3f3a0934f3a5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440910"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageFileCounts(period='D7')')
    .version('beta')
    .get();

```