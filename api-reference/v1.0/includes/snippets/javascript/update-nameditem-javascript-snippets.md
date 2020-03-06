---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 333a8fe65a6e107c7bd15ee61d7c9de4bd8f3373
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636816"
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
    .update(workbookNamedItem);

```