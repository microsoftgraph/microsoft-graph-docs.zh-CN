---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 12e6fc9eafa76f4c5230d40f0a6ab3d296c46a43
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480153"
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