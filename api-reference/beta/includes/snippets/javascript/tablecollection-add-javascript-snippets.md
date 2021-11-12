---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10a94d6b8303b2020b50441c99ff33b9c8320a1beb63e743cad818910c81c356
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: 'Sheet1!A1:D5',
  hasHeaders: true
};

await client.api('/me/drive/items/{id}/workbook/tables/add')
    .version('beta')
    .post(workbookTable);

```