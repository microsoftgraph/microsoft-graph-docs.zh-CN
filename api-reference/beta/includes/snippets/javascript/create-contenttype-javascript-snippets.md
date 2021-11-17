---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 725ed271502235f7a5981410a5bdba5c0c91a5042e753d2f2a9ad00a2813f193
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163070"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contentType = {
    name: 'docSet',
    description: 'custom docset',
    base: {
        name: 'Document Set',
        id: '0x0120D520'
    },
    group: 'Document Set Content Types' 
};

await client.api('/sites/{id}/contentTypes')
    .version('beta')
    .post(contentType);

```