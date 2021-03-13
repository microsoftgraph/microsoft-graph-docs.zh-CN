---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d7ababb5ad281798448b494893f6d48d744e8d6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805119"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reviewSetQuery = {
   displayName: 'My Query 1',
   query: '(subject:\"Quarterly Financials\")'
};

await client.api('/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries')
    .version('beta')
    .post(reviewSetQuery);

```