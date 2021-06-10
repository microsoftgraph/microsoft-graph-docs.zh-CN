---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 441aaeff91543e7bd4c80306b446b81c9f1df39f
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dailyPrintUsageByUser = await client.api('/print/reports/dailyPrintUsageByUser')
    .version('beta')
    .get();

```