---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f909cd1bf1e4e8a21f1d41abe1d4ad89f2d17cb3daa7419bbe41ea9bae20059b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378598"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let temporaryAccessPassAuthenticationMethod = await client.api('/users/kim@contoso.com/authentication/temporaryAccessPassMethods/30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30')
    .version('beta')
    .get();

```