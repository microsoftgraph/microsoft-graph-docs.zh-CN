---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1bf8e63c7a62c1bf5484c7ef27c3752ee101dbf9c2fb3312170cba85439ac2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/kim@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2')
    .version('beta')
    .delete();

```