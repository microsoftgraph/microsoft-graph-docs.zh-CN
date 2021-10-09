---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e560092cf7c43ae85a4d8000fe78fdbb3fce105597e53f544f4a2d533540d8e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    '@odata.id':'https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2'
};

await client.api('/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref')
    .version('beta')
    .post(directoryObject);

```