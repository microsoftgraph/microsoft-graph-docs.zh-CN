---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 599ff3e247c437eb8ee59818b7c3afa1b7ddba7940dfc54058f963b596f10d77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220928"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oAuth2PermissionGrant = await client.api('/oauth2PermissionGrants/{id}')
    .get();

```