---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 14f2a6b1f720b25874e16fe65fde307d959cd0ac
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsagePages(period='D7')')
    .version('beta')
    .get();

```