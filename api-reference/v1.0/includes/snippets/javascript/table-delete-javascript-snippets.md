---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a584c391dc17619da06d920998c6d29e67dc4f6a92041c67cfa4d614d1a0b225
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}')
    .delete();

```