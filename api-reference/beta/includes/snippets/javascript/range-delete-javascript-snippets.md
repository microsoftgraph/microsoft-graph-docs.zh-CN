---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42d52fd8d4de402484b51ec03349814808273b27a747fca381ba401aeff17fac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221507"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _delete = {
  shift: 'shift-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/delete')
    .version('beta')
    .post(_delete);

```