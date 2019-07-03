---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fbaca6101a75ab8a75ef4f9a308443c37f5d5220
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageStorage(period='D7')')
    .version('beta')
    .get();

```