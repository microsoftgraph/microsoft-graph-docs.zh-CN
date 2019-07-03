---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3a22207a0c999cab19d39407649cc12fa23f2a9a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/items/{item-id}/permissions/{perm-id}')
    .version('beta')
    .delete();

```