---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb25f1360fe346df752e93ab70375326fcc7c83d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615608"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/joinedTeams')
    .version('beta')
    .get();

```