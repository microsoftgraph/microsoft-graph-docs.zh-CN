---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6823d2247842db96757d2ac8f782c8586e396bd07c24138c757829ce4a1db7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104288"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rows = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .skip(5)
    .top(5)
    .get();

```