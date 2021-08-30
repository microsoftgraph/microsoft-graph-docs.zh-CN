---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42b2c00b9aa3c0ce3b243079d8c209b726b10c1ea73491c235532ae83ccd8e18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158471"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/servicePrincipals/{id}/oauth2PermissionGrants')
    .version('beta')
    .get();

```