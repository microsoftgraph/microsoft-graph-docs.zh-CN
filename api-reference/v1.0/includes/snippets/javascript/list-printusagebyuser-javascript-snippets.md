---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 380f495a8fdb2b0fab2554e2ac219fa303cf319c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768720"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageByUser = await client.api('/reports/monthlyPrintUsageByUser')
    .get();

```