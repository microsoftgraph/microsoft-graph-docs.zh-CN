---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ce84456ebad31c233ae5b2fc495fcf5dfcd60bdfc56e1f9db1c2be9d535bfd4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219104"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/LastRow')
    .version('beta')
    .get();

```