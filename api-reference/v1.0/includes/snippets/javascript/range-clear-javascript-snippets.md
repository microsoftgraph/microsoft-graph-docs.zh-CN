---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f714c3b3f728a8b73cd558663d37d5ac1883ffb36ae112d8399f619e1b327d7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409482"
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
    .post(clear);

```