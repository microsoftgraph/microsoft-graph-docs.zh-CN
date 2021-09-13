---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6abb25fa556ec53dfc210cb01cfd53cb18a51f6fa251308081105db6b5e63706
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/planner/plans')
    .get();

```