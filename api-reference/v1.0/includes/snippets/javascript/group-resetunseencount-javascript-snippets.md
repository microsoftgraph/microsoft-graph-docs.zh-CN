---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b8bc9a03b4630f06da6538c1aa7e8e8be238deabee499f33bfafcdc284927a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220993"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/resetUnseenCount')
    .post();

```