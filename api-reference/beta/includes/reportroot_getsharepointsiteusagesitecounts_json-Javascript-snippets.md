---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 12e6fc9eafa76f4c5230d40f0a6ab3d296c46a43
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464697"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageSiteCounts(period='D7')')
    .version('beta')
    .get();

```