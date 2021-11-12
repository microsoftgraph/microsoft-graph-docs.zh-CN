---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc1a9a8962a0d394b1b4566c81677b9e312f027f4c370c11e92f2c780c6e301f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rows = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .version('beta')
    .skip(5)
    .top(5)
    .get();

```