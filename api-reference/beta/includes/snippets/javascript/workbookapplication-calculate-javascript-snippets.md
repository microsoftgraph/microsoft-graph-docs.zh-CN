---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 274b28e25881b97459bc1b15082ad16b302593d9511261cd08d046b7c79e8ff9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calculate = {
  calculationType: 'calculationType-value'
};

await client.api('/me/drive/items/{id}/workbook/application/calculate')
    .version('beta')
    .post(calculate);

```