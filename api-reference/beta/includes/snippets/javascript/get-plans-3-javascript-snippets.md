---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cbef6e3e1fa8231321a98725173f584d009184b82920e5e0e900378c71bed7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/me/planner/plans')
    .version('beta')
    .get();

```