---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0aa57ca7c59672ce6b001da20395073259eabffe
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange')
    .version('beta')
    .get();

```