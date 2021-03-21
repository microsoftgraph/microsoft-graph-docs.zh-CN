---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d324d220bf790635722eb7a4ec64da1f8b78a2f6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageSummariesByPrinter = await client.api('/print/reports/monthlyPrintUsageSummariesByPrinter')
    .version('beta')
    .get();

```