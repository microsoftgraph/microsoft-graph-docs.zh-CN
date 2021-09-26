---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b167577972d6757fb429879e964c33fbf854b9e34133adc02f658ecb4bb057b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/oauth2PermissionGrants')
    .version('beta')
    .get();

```