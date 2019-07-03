---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6e21993ba254f40e01a81227cd3a2beb3a2c7e39
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageStorage(period='D7')')
    .get();

```