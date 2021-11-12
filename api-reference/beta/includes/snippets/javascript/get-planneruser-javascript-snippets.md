---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ee7da65495f3f6817d02dbbecf81e8e895f2e9d67a152a1dc0c78d34331f5c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218469"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerUser = await client.api('/me/planner')
    .version('beta')
    .get();

```