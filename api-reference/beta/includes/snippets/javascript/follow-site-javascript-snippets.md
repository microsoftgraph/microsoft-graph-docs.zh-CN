---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2c782ff5a1fc746fd14daca32bde1a11d2e0f16
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const site = {
    value: 
    [
        {
            id: 'contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740'
        },
        {
            id: 'contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851'
        }
    ] 
};

await client.api('/users/{user-id}/followedSites/add')
    .version('beta')
    .post(site);

```