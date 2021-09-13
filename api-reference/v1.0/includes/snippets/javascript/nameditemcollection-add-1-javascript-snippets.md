---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecfb2fe971a539fe8b448ca8bee6f8b26f0ec3fce8bb4dc8cc0f7370fc90b29c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  name: 'test5',
  reference: '=Sheet1!$F$15:$N$27',
  comment: 'Comment for the named item'
};

await client.api('/me/drive/items/{id}/workbook/names/add')
    .post(workbookNamedItem);

```