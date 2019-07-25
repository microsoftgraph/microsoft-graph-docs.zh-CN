---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fbaca6101a75ab8a75ef4f9a308443c37f5d5220
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718958"
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