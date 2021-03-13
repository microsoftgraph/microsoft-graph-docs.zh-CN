---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a08379f0f3e2bb1b3ee3fc01f39ad65b1c8df296
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printUsageByPrinter = await client.api('/print/reports/dailyPrintUsageSummariesByPrinter/{id}')
    .version('beta')
    .get();

```