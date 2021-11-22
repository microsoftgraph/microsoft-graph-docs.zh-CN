---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ab2df7c15c8cb7c7be7423ea4568b340fab715d00a1e468aeeda54ed03b56d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164072"
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