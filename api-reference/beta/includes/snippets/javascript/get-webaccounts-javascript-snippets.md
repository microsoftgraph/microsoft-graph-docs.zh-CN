---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d1e2632d12c2c6aa118cf2fa997b2d43ee924f62969f71da0e0429a0c141654
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221077"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let webAccounts = await client.api('/me/profile/webAccounts')
    .version('beta')
    .get();

```