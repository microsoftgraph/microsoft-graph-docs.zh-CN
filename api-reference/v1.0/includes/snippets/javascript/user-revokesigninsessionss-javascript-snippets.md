---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d293ef099cfb7e002a3d1d404e21d67c0911014283c801f51d629bd7d607aa25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106753"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/revokeSignInSessions')
    .post();

```