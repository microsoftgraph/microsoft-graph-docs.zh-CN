---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0d2e80c9eeaaadf5abe34d1f49a846b932ecf2f6a8329a1de93bd213fef529a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .version('beta')
    .get();

```