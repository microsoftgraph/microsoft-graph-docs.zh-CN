---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 530015cb2d950c11ce3beb4ee363919b083771f3a80c110f07e3c444bb970c57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookWorksheet = {
  position: 99,
  name: 'name-value',
  visibility: 'visibility-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .update(workbookWorksheet);

```