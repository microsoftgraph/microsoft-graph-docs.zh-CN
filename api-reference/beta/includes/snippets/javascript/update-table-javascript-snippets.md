---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f35748d82db9bb78b1fcd3102ecca1d8a9119922a5679f5d547f56ff9411338f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163353"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  name: 'name-value',
  showHeaders: true,
  showTotals: true,
  style: 'style-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}')
    .version('beta')
    .update(workbookTable);

```