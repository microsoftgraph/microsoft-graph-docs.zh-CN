---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c47ceec2a1ca07c2b73137df7cf8be08dc9e9eee38b5e1d1bcf93c57783c3198
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273830"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect')
    .post();

```