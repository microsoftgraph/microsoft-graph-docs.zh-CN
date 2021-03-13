---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f68510a2a845f310a0239c7a0b242eba4bfbd725
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784019"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let reviewSetQuery = await client.api('/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807')
    .version('beta')
    .get();

```