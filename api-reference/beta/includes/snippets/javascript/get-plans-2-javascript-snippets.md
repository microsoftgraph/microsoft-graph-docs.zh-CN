---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f8e8a4660dcbd6a5e05fcaec87dcd643f8d6d3c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945939"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/groups/ebf3b108-5234-4e22-b93d-656d7dae5874/planner/plans')
    .version('beta')
    .get();

```