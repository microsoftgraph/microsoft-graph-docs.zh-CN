---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb7cff0a5d325baa456bbd5192dcc32835ec195b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/account/{id}')
    .version('beta')
    .delete();

```