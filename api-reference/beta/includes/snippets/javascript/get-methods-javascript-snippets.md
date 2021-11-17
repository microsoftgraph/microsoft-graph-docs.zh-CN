---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 262c62ade560c564f0766244645d90f7a25f3b1f6f3c6412f0adee1aa818b744
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let methods = await client.api('/me/authentication/methods')
    .version('beta')
    .get();

```