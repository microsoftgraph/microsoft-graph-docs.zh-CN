---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba6bbf0bf1063463b72a2eada2a3758731fbeead81c976e13202e497ec93cc8f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106263"
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

await client.api('/users/{user-id}/followedSites/remove')
    .version('beta')
    .post(site);

```