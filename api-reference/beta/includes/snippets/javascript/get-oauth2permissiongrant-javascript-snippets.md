---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdfe3d96d512c5854ac8555a08b9114a5604a01e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oAuth2PermissionGrant = await client.api('/oauth2PermissionGrants/AVs6JuUDjkCFV7q2gd8QTPimBBgj5iBFj0C6GwwRxC0')
    .version('beta')
    .get();

```