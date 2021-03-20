---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03693acadebb12ede0047234e3cecd1e0b928a09
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952837"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tables = await client.api('/me/drive/items/{id}/workbook/tables')
    .version('beta')
    .get();

```