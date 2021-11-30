---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44716246f2bbd8843389d69e80aef640d5d8459b
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226205"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
    customSecurityAttributes: 
    {
        Engineering: 
        {
            '@odata.type':'#Microsoft.DirectoryServices.CustomSecurityAttributeValue',
            ProjectDate: '2022-10-01'
        }
    }
};

await client.api('/servicePrincipals/{id}')
    .version('beta')
    .update(servicePrincipal);

```