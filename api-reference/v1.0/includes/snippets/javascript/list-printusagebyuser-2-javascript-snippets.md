---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d68e3596622d596df03ca151c8c4796f1203fa22e58d1401307c526568511ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378250"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageByUser = await client.api('/reports/monthlyPrintUsageByUser')
    .get();

```