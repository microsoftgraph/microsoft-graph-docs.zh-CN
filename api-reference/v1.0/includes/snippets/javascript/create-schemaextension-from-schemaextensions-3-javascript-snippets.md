---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c7b1d2cbf1ffde2ef8112f4c7cdeaaf3c6fa5883a3a108e4f3bb3734b5346da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
    id: 'courses',
    description: 'Graph Learn training courses extensions',
    targetTypes: [
        'Group'
    ],
    owner: '50897f70-a455-4adf-87bc-4cf17091d5ac',
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
    .post(schemaExtension);

```