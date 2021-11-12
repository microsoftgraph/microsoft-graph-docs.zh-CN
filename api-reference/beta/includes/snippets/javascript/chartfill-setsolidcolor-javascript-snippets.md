---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fde195d03ebc53d92763c4d198c880dcff57a1aeb52885eadb2204d2bc55c8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273816"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setSolidColor = {
  color: 'color-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor')
    .version('beta')
    .post(setSolidColor);

```