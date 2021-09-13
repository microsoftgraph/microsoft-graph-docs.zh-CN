---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14824d756ea2d173c1c613a4ee987956e5408e15175795c706a718830906a694
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/oauth2PermissionGrants/{id}')
    .delete();

```