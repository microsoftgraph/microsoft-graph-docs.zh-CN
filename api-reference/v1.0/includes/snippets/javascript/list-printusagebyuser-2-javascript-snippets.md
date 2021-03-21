---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 380f495a8fdb2b0fab2554e2ac219fa303cf319c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959554"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageByUser = await client.api('/reports/monthlyPrintUsageByUser')
    .get();

```