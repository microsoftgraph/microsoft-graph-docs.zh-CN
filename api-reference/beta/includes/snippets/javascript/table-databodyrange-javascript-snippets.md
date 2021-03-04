---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: beb251be16fdb0ef5d57526aa5563171cdcc073f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/DataBodyRange')
    .version('beta')
    .get();

```