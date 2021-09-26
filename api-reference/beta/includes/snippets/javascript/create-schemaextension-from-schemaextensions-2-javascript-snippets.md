---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fcf43d217e70cc47ff8ab37c5dadaa1f35185e27354e7a5626b0e138bbc4855
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158483"
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