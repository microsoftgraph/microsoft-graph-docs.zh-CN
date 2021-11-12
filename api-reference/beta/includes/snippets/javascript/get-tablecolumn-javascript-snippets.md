---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec7cf32372254369ec1f1da7ddd6fa658831b0dac2dde7f2a7ed624fe5a7b4c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378615"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableColumn = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}')
    .version('beta')
    .get();

```