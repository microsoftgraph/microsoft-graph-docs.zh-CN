---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea2ec55dc491c8c899243fd019a069bc5b0206ee
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
    owner: 'ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa',
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
        },
        {
            name: 'courseSupervisors',
            type: 'String'
        }
    ]
};

await client.api('/schemaExtensions/exto6x7sfft_courses')
    .update(schemaExtension);

```