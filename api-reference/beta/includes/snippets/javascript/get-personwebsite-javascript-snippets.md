---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ba0193cb6011f1093cfb3f8dd104d0a1a0dc9384152faef26109f88eb43624e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220499"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personWebsite = await client.api('/me/profile/websites/{id}')
    .version('beta')
    .get();

```