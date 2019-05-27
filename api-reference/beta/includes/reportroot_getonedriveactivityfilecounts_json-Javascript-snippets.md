---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8011b988e8440c14c312dd0533053f9e388c9d47
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441211"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveActivityFileCounts(period='D7')')
    .version('beta')
    .get();

```