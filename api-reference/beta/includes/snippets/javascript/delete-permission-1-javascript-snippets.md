---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7ac8192f3dbfb7b189dba0c0fcc71a15842f9aa56b806013e3a09a212575352
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277425"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .version('beta')
    .delete();

```