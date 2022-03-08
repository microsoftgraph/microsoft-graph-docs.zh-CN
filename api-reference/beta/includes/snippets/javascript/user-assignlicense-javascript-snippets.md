---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d90877ac28a363cd6df999e60714fd94ea4b84bf
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339964"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
    addLicenses: [
        {
            disabledPlans: [
                '8a256a2b-b617-496d-b51b-e76466e88db0'
            ],
            skuId: '84a661c4-e949-4bd2-a560-ed7766fcaf2b'
        },
        {
            disabledPlans: [],
            skuId: 'f30db892-07e9-47e9-837c-80727f46fd3d'
        }
    ],
    removeLicenses: []
};

await client.api('/me/assignLicense')
    .version('beta')
    .post(user);

```