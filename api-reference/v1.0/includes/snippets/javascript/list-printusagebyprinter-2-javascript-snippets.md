---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0cdc7a2f41bc38e8aedd51e07003abbe941b4a5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959590"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let monthlyPrintUsageByPrinter = await client.api('/reports/monthlyPrintUsageByPrinter')
    .get();

```