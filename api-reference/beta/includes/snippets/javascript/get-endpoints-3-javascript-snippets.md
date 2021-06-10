---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ed1615db8d07a9af6faba003370a263cebb9ff1
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871521"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dailyPrintUsageByPrinter = await client.api('/print/reports/dailyPrintUsageByPrinter')
    .version('beta')
    .get();

```