---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ae126f3bbc177badef56d9a2371894ee73b213e726f2056bab53e59c54db46a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328843"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedObjects = await client.api('/me/ownedObjects')
    .get();

```