---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30c43b9a641e8bc6c99547d862ebb6901daa64f2ebf2e15f40cae80dd7ec32c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219074"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/conditionalAccess/policies/{id}')
    .version('beta')
    .delete();

```