---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ce018451b1cdbc901945c2d3527650230cdc48ad6cccd1bd9ea8af5db5c03eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: 'john@contoso.com'
    },
    {
      email: 'ryan@external.com'
    }
  ],
  roles: ['read']
};

await client.api('/shares/{encoded-sharing-url}/permission/grant')
    .version('beta')
    .post(permission);

```