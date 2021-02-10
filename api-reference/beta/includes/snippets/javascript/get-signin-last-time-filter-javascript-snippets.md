---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3caf77a2af2aaacfab983a3876463ad190c3102b
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179154"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .version('beta')
    .filter('startswith(displayName,'Eric')')
    .select('displayName,signInActivity')
    .get();

```