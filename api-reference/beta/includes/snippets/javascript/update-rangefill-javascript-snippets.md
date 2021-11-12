---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d55a1ee908df287a20d87c1c42ba7f625d6a11e1ba2b7fbff6daf1b28220ce5c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: 'color-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .version('beta')
    .update(workbookRangeFill);

```