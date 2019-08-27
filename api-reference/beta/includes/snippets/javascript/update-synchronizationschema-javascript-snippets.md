---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83d53fbfb7c386a3d6911b74107df3c0f6dfab7a
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationSchema = {
    directories: [
        {
            name: "Azure Active Directory",
            objects: [
                {
                    name: "User",
                    attributes: [
                        {
                            name: "userPrincipalName",
                            type: "string"
                        }
                    ]
                },
            ]
        },
        {
            name: "Salesforce",
        }
    ],
    synchronizationRules:[
        {
            name: "USER_TO_USER",
            sourceDirectoryName: "Azure Active Directory",
            targetDirectoryName: "Salesforce",
            objectMappings: [
                {
                    sourceObjectName: "User",
                    targetObjectName: "User",
                    attributeMappings: [
                        {
                            source: {},
                            targetAttributeName: "userName"
                        },
                    ]
                },
            ]
        },
    ]
};

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema')
    .version('beta')
    .put(synchronizationSchema);

```