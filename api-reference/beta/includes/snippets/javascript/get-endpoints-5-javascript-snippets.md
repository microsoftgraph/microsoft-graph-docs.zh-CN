---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63e5696ee28ee6f4c936a965b0a51d7273e3b6d1
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageByPrinter = await client.api('/print/reports/monthlyPrintUsageByPrinter')
    .version('beta')
    .get();

```