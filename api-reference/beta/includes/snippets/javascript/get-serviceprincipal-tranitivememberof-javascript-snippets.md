---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db00c9e8de13495fbf5d28ff960dadaf28e9ab49
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/servicePrincipals/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```