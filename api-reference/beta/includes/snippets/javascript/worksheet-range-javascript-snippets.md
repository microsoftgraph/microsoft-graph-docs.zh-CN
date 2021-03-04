---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b0550841c83fb991e885ee33cf3d1d943855e35
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444570"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/Range')
    .version('beta')
    .get();

```