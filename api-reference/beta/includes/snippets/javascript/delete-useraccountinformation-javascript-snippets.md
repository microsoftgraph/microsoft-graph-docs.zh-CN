---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40e0441fcc12aaca21043c5beaaada092be0d119bb77fed3f55348d46beb8f84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278656"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/account/{id}')
    .version('beta')
    .delete();

```