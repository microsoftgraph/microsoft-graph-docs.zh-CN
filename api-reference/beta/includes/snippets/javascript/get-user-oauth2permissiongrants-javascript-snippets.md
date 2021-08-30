---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbe530ef37cf130283ee7f98855810f46525289da040a82a87e12b26044b6666
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218831"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/oauth2PermissionGrants')
    .version('beta')
    .get();

```