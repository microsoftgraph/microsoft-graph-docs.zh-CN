---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9658d0af3ef1094662bdfbfe4826068fa7da911e5adf2223eca8fa3a37d25397
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273965"
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