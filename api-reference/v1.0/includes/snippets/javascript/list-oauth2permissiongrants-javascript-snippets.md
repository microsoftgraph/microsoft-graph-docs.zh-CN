---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec8ea3ce0f2f0e17fe98144a5658e9a847f7ee1d28577bc4621d62244e3662e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278521"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/oauth2PermissionGrants')
    .get();

```