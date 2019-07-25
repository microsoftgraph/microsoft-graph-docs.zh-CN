---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5c7952c9af82743ea730b06cb3df7f9f31c7de58
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageDetail(period='D7')')
    .get();

```