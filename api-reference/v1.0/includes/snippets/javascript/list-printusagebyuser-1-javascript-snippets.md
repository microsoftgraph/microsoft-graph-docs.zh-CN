---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d255731e461fe1c9cc687ce71eaa7d464171ffaee7df4d4cbff1284f4488d5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dailyPrintUsageByUser = await client.api('/reports/dailyPrintUsageByUser')
    .get();

```