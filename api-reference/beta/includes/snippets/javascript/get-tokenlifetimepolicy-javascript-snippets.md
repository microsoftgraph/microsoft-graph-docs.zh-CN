---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72291b933c1355b8b4aac4fe3c643f5fc8f2799beaf1084fc0548fe7a4c520ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenLifetimePolicy = await client.api('/policies/tokenLifetimePolicies/{id}')
    .version('beta')
    .get();

```