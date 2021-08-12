---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a477303ae5b8c3feb11256e5bd4c2ad681b7495dfc345302fbab1143f1583492
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54275135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageByUser = await client.api('/print/reports/monthlyPrintUsageByUser')
    .version('beta')
    .get();

```