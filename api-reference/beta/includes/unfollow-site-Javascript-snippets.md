---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 14b4247ece85a21753a2045346e2d07060ff48f8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330031"
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
    .version('beta')
    .post(site);

```