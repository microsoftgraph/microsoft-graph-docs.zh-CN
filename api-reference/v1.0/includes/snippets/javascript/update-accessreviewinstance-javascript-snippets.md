---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cfa9c51df391677950cbbed3e38ca3627d0f21d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095446"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewInstance = {
    scope: {
        '@odata.type': '#microsoft.graph.principalResourceMembershipsScope',
        principalScopes: [
            {
                '@odata.type': '#microsoft.graph.accessReviewQueryScope',
                query: '/v1.0/users',
                queryType: 'MicrosoftGraph'
            },
            {
                '@odata.type': '#microsoft.graph.accessReviewQueryScope',
                query: '/v1.0/groups',
                queryType: 'MicrosoftGraph'
            }
        ],
        resourceScopes: [
            {
                '@odata.type': '#microsoft.graph.accessReviewQueryScope',
                query: '/beta/roleManagement/directory/roleDefinitions/9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3',
                queryType: 'MicrosoftGraph'
            }
        ]
    },
    reviewers: [
        {
            query: '/users/1ed8ac56-4827-4733-8f80-86adc2e67db5',
            queryType: 'MicrosoftGraph'
        }
    ],
    fallbackReviewers: [
        {
            query: '/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e',
            queryType: 'MicrosoftGraph'
        },
        {
            query: '/users/1ed8ac56-4827-4733-8f80-86adc2e67db5',
            queryType: 'MicrosoftGraph'
        }
    ]
};

await client.api('/identityGovernance/accessReviews/definitions/5dcfcc88-da88-4252-8629-a0807b4b076d/instances/720b8ee0-cee4-42ac-b164-894c48703acc')
    .update(accessReviewInstance);

```