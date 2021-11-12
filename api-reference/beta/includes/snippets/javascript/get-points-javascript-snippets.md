---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 605b161cbdd7f76b536eb7b0db1806f2cb9ff3fcd5bd3d47900791202256b4c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let points = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points')
    .version('beta')
    .get();

```