---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85721847e9d52f5916a6cb97b035d06ac4772cecce2ce6f58425e0e5a80ce1a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409520"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let microsoftAuthenticatorAuthenticationMethod = await client.api('/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2')
    .get();

```