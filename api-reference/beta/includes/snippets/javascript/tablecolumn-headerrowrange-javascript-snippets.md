---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2156c97e48b05c6e7b30555813baa744c85f466f5de5ee32d39454a71b8b3a74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/HeaderRowRange')
    .version('beta')
    .get();

```