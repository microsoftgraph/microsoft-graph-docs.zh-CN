---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b08eaf883ae52658030eddb84bc83a572f3a421dacb25d1db56c6491a33ac20d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279570"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/TotalRowRange')
    .version('beta')
    .get();

```