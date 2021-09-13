---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb60b2d4cec67cc1ae4ceb17eddb663a09e632ac90e778e2741ed8bc4fea6168
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .delete();

```