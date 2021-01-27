---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5770b58fa7f23a88740ca46b39e20006332b68a
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/reports/dailyPrintUsageSummariesByPrinter')
    .version('beta')
    .get();

```