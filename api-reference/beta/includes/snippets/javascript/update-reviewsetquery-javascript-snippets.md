---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce608486278221714eeef046cb9a99ee436a5258
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772785"
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