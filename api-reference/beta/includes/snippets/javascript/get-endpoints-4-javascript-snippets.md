---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c43213c7b7166e2d8ca68c302f2120f48a9e80a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953069"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dailyPrintUsageSummariesByUser = await client.api('/print/reports/dailyPrintUsageSummariesByUser')
    .version('beta')
    .get();

```