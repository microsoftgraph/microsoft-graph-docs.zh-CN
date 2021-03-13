---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5b1c27c242cd616214996aa985aafe1b0e98906
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationSchema = {
    directories: [
        {
            name: 'Azure Active Directory',
            objects: [
                {
                    name: 'User',
                    attributes: [
                        {
                            name: 'userPrincipalName',
                            type: 'string'
                        }
                    ]
                },
            ]
        },
        {
            name: 'Salesforce',
        }
    ],
    synchronizationRules: [
        {
            name: 'USER_TO_USER',
            sourceDirectoryName: 'Azure Active Directory',
            targetDirectoryName: 'Salesforce',
            objectMappings: [
                {
                    sourceObjectName: 'User',
                    targetObjectName: 'User',
                    attributeMappings: [
                        {
                            source: {},
                            targetAttributeName: 'userName'
                        },
                    ]
                },
            ]
        },
    ]
};

await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema')
    .version('beta')
    .put(synchronizationSchema);

```