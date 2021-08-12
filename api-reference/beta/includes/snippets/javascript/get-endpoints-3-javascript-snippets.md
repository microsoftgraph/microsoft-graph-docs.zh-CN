---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9779df9887513d4b2b05f06c96ee750ebdb94670eebac75785d814bbb1349c1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54275559"
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