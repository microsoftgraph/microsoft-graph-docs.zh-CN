---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0374c4c2e8d5ee3c78cd720052248db5caeddc6313b24b56bb47ce5f70766ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/range')
    .get();

```