---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 626b5c1f03873b2bcb1daa4ed7ee9ba29992c834
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682210"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/dataBodyRange')
    .get();

```