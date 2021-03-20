---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de7148f4a69e07046392bb960a1f26b92726e58b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dailyPrintUsageByPrinter = await client.api('/reports/dailyPrintUsageByPrinter')
    .get();

```