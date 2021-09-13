---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a44810f89e5d43390fed067343784aa7b327a0ad23e0ee1571e85eb1aba21e7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409350"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryRole = {
  roleTemplateId: 'fe930be7-5e62-47db-91af-98c3a49a38b1'
};

await client.api('/directoryRoles')
    .post(directoryRole);

```