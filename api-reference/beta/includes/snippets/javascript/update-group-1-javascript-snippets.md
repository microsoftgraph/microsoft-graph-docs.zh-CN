---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 758c30f95f65a4218598eba34fb57d625767f0da88f1c9bdb034cb0aff983a93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277436"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
   description: 'Contoso Life v2.0',
   displayName: 'Contoso Life Renewed'
};

await client.api('/groups/{id}')
    .version('beta')
    .update(group);

```