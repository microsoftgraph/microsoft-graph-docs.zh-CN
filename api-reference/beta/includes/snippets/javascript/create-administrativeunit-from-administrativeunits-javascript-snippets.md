---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea4012549fffbe042d0d333bd8bcfe07c16f777822a2a02b45a3056086ca88ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
    displayName: 'Seattle District Technical Schools',
    description: 'Seattle district technical schools administration',
    visibility: 'HiddenMembership'
};

await client.api('/administrativeUnits')
    .version('beta')
    .post(administrativeUnit);

```