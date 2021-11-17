---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb32bdc698ca50ccfa146e0aa3940d9647f6e285364e109f9db1c4e4ac6dc761
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106851"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeCard = await client.api('/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972')
    .version('beta')
    .get();

```