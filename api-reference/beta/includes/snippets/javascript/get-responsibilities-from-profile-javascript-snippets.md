---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d09f274468927a0e48cf5398acee9bc0b600daed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/responsibilities')
    .version('beta')
    .get();

```