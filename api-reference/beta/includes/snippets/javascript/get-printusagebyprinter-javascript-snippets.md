---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c7d87a5bda2540e846d97c179e46fc6397ca41cfe75733ef8a54b49f5172294
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221082"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printUsageByPrinter = await client.api('/print/reports/dailyPrintUsageByPrinter/016b5565-3bbf-4067-b9ff-4d68167eb1a6')
    .version('beta')
    .get();

```