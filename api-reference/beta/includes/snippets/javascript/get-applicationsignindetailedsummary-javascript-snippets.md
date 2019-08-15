---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 476813818cfb7f4bb9c3b37fad4781c0d733d5ea
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/applicationSignInDetailedSummary/{id}')
    .version('beta')
    .get();

```