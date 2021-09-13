---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7ed84ee7234de168516bdee0737f4ecb5aa6b7e2300363a1113f5bc51bac0e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
  properties: [
    {
      name: 'new-name-value',
      type: 'new-type-value'
    },
    {
      name: 'additional-name-value',
      type: 'additional-type-value'
    }
  ]
};

await client.api('/schemaExtensions/{id}')
    .update(schemaExtension);

```