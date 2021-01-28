---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea9b069b41b92c0e33a3c2dcb6ded8981ee7b02a
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  name: "test5",
  reference: "=Sheet1!$F$15:$N$27",
  comment: "Comment for the named item"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/add')
    .post(workbookNamedItem);

```