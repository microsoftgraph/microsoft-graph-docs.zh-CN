---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5644ebce3948966005c7c2ce4d022cc36b44dfa4c90369f5c34369068228ef4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220969"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear')
    .post();

```