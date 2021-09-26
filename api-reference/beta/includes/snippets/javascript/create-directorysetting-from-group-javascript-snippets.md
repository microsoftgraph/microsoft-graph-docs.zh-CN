---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cfa54f41f72bbb241a5a6b00b069aa3d1ee7dbf3478908eba120c324f9ba581
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  directorySetting: {
    displayName: 'displayName-value',
    templateId: 'templateId-value',
    values: [
      {
        name: 'name-value',
        value: 'value-value'
      }
    ]
  }
};

await client.api('/groups/{id}/settings')
    .version('beta')
    .post(directorySetting);

```