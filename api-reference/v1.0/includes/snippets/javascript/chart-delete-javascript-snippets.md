---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4667eddfe4d2104b3e2ae3ec7a3eb8766609e9430b80b1bf9942872ed45c1039
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}')
    .delete();

```