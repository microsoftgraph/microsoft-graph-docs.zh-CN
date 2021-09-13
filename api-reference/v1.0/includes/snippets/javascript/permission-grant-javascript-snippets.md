---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52a00f147587a0b855d8dc3350334a30642945aaa290e23dc9caf1b72c5f5549
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162561"
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
    .post(permission);

```