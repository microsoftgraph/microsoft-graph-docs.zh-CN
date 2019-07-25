---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8271891c1fd6931316c0f0e561ed0fe38754507d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  type: "type-value",
  scope: "scope-value",
  comment: "comment-value",
  value: {
  },
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .version('beta')
    .update({workbookNamedItem : workbookNamedItem});

```