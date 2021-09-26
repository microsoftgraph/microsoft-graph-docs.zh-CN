---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14e91dd5e14c52afbbb3f4ecfe44b89353d06ac4a875afa21bf53b6c72ee2622
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
    id: 'graphlearn_courses',
    description: 'Graph Learn training courses extensions',
    targetTypes: [
        'Group'
    ],
    properties: [
        {
            name: 'courseId',
            type: 'Integer'
        },
        {
            name: 'courseName',
            type: 'String'
        },
        {
            name: 'courseType',
            type: 'String'
        }
    ]
};

await client.api('/schemaExtensions')
    .version('beta')
    .post(schemaExtension);

```