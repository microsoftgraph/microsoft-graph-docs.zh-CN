---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62739b3b2f1eca2a1d86f41231a256e25702f3690060bcdc87ff8f90ae998dec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104735"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schedule = await client.api('/teams/{teamId}/schedule')
    .version('beta')
    .get();

```