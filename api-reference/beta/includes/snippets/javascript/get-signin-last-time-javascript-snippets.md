---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aee7b1b0f6a1932928a3458672f529b9430a9462
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41778041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .version('beta')
    .select('displayName,userPrincipalName,signInActivity')
    .get();

```