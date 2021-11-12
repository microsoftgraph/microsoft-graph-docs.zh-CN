---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52d2be9a92027223366eb665172a1255ea0a2479d8d079ec191d22bf7d6ded94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let names = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/names')
    .version('beta')
    .get();

```