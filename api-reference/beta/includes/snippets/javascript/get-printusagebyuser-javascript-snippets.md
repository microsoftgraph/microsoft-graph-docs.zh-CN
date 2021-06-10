---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83e32e3385462fd02b4a93a6145517274f9e9652
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printUsageByUser = await client.api('/print/reports/dailyPrintUsageByUser/016b5565-3bbf-4067-b9ff-4d68167eb1a6')
    .version('beta')
    .get();

```