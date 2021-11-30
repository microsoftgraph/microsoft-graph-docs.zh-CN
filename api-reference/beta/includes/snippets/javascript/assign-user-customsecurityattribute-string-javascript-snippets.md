---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: caae7b960be7d9db4e68c37cfe57f9b1a70b1d7d
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
    customSecurityAttributes: 
    {
        Engineering: 
        {
            '@odata.type':'#Microsoft.DirectoryServices.CustomSecurityAttributeValue',
            ProjectDate: '2022-10-01'
        }
    }
};

await client.api('/users/{id}')
    .version('beta')
    .update(user);

```