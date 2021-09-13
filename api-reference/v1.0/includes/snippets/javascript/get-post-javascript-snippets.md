---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3534c7175692eee2996d098d98088786727d26280d4a5acdfd4d1287fa00ba14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158336"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let post = await client.api('/groups/{id}/threads/{id}/posts/{id}')
    .get();

```