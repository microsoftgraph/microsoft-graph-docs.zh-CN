---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d7aadb9f03ba6065a7c0cce402b6146e880762e2118b5462dedb1b4a9987b6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const apply = {
  fields: [
    {
      key: 99,
      sortOn: 'sortOn-value',
      ascending: true,
      color: 'color-value',
      dataOption: 'dataOption-value',
      icon: {
        set: 'set-value',
        index: 99
      }
    }
  ],
  matchCase: true,
  method: 'method-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply')
    .version('beta')
    .post(apply);

```