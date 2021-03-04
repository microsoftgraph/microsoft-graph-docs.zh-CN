---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6572870f0efc3eaffbb2722fdc71b092427796a9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/reports/dailyPrintUsageSummariesByUser/{id}')
    .version('beta')
    .get();

```