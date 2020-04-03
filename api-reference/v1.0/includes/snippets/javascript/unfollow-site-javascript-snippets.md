---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af93636f268a362413762b6204ceabe29eeda035
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125048"
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
            id: "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740"
        },
        {
            id: "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851"
        }
    ] 
};

let res = await client.api('/users/{user-id}/followedSites/remove')
    .post(site);

```