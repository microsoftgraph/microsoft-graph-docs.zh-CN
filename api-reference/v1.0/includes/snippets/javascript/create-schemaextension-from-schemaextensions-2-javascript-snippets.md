---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fb95ce99a8052c37a8ddc3f47d07cb6b3cb782fd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509059"
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
    .post({schemaExtension : schemaExtension});

```