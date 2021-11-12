---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a56336be783da0ae7086dcc7e74388ad4c9680f241c94e6a7849b0b29ede2a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .version('beta')
    .skip(5)
    .top(5)
    .get();

```