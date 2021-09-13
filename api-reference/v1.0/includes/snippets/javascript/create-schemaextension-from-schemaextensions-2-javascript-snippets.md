---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf0c04cfc4f83b3e97f2145008434f642fcf0e92e0d0592cb3354abcd4b902fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219295"
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
    .post(schemaExtension);

```