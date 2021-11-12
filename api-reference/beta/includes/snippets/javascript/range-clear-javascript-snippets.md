---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b2b005e201c86a225635d7531aaa7fa17d9b64f8debc5bef225ea98538377ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106500"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clear = {
  applyTo: 'applyTo-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/clear')
    .version('beta')
    .post(clear);

```