---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45b963717647dd999716a6eb1d73595585af8c7a9475dc4fcb4d486d4bde8f37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277380"
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
    .version('beta')
    .update(workbookWorksheet);

```