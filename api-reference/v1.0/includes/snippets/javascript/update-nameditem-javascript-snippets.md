---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f6b06eccb65df14722b6d7e5e69cc9055745ca33d38508ed660efa649dd57a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161609"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  type: 'type-value',
  scope: 'scope-value',
  comment: 'comment-value',
  value: {
  },
  visible: true
};

await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .update(workbookNamedItem);

```