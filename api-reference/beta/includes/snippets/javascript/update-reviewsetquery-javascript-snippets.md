---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e93919e8f79172698d301ba04db15e5f424bb2bf01e42eddb82e7050ad86533
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161709"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reviewSetQuery = {
  displayName: 'My Query 1 - Renamed'
};

await client.api('/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807')
    .version('beta')
    .update(reviewSetQuery);

```