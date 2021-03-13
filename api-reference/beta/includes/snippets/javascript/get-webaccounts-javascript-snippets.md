---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1081961e31f51955cb98cf502315fc05d6c71e46
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779085"
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