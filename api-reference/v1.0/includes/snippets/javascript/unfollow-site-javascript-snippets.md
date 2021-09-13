---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 129b516fb727f43a7f07374883001836b2e90408657c389fa52a3fed391b4749
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101305"
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
    .post(site);

```