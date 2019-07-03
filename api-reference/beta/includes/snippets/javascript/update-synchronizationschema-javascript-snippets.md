---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 34f3cc862a7c348c9297171258c85a174905cf20
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500523"
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
    .put({synchronizationSchema : synchronizationSchema});

```