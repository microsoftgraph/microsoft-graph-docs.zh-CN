---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1463d229df54a5e02bdd8ccd4183e03ecd9ef9a4a94f3a74a54ef900c19ac9ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161496"
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