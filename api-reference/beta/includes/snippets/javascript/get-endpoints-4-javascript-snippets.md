---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 066a5e0c1750c93ef2a3c0ea8eecaa6ddca058c53ba1381026f63b946161b44d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54275489"
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