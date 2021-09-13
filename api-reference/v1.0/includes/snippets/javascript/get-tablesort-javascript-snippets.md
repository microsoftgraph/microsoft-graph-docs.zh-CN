---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 472d4a0a56b47f0a2da7be572fb246aa92c0e86722628e2820eeff500c7fb487
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378315"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableSort = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort')
    .get();

```