---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82d13c253f470983e64373b904c8f0e1076e2f9bcf5d05c465a2c4470b018298
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162523"
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
    .post(calculate);

```