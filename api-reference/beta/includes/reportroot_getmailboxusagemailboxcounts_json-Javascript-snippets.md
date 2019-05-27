---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e22b8dfec22959c7996e64356eae190434a7ea7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441967"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageMailboxCounts(period='D7')')
    .version('beta')
    .get();

```