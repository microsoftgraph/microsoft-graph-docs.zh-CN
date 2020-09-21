---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24bc706f7e1ad7f118323cc0a29d22c0645b58d6
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565085"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reviewSetQuery = {
     "displayName" : "My Query 1",
     query: "(subject:\"Quarterly Financials\")"
};

let res = await client.api('/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries')
    .version('beta')
    .post(reviewSetQuery);

```