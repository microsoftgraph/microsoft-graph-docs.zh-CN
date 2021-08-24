---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79e2385198b6df6b44899210d918804bc8d8160c0ebdd040618481575dcc89a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218940"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/groups/delta')
    .version('beta')
    .select('displayName,description,mailNickname')
    .get();

```