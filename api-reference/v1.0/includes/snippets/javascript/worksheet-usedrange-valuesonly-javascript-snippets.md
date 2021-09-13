---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e195b878fc7ad5497621277535a4574f856415232f7615e066451c16187fb8b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219082"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)')
    .get();

```