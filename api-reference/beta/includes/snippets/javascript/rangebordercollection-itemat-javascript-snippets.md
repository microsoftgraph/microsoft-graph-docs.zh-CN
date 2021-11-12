---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a048e0844e073787a4d6caa4e22cecc95034b98c11f6caac44286953b36b884a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158495"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  index: {
  }
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/ItemAt')
    .version('beta')
    .post(workbookRangeBorder);

```