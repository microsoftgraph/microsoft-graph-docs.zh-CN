---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 165c9c4be73c2e7a5eb59f10fae680e9265b3d166b31238d1007ac385d6d383e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedObjects = await client.api('/me/ownedObjects')
    .version('beta')
    .get();

```