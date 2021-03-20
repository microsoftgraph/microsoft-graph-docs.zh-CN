---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3312be8c4e0b36c254b4f4e8a3119169cda8fe34
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/planner/rosters/6519868f-868f-6519-8f86-19658f861965/plans')
    .version('beta')
    .get();

```