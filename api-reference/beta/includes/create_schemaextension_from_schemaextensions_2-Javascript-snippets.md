---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6603766d1751956e8eb4f8c6c2ff08847a36679a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
    id:"courses",
    description: "Graph Learn training courses extensions",
    targetTypes: [
        "Group"
    ],
    properties: [
        {
            name: "courseId",
            type: "Integer"
        },
        {
            name: "courseName",
            type: "String"
        },
        {
            name: "courseType",
            type: "String"
        }
    ]
};

let res = await client.api('/schemaExtensions')
    .version('beta')
    .post({schemaExtension : schemaExtension});

```