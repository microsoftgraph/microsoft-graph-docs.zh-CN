---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ccb3b430dc815503fec5bfc69ba6002be9ef208
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61076986"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/users/{id | userPrincipalName}')
    .select('displayName,givenName,postalCode,identities')
    .get();

```