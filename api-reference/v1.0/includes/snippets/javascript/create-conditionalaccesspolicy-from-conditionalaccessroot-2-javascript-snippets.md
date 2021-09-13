---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e63c9d694026a216ed37ab9b3bdc3f71809f0bf11e385d23f9761419f410badf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    displayName: 'Block access to EXO non-trusted regions.',
    state: 'enabled',
    conditions: {
        clientAppTypes: [
            'all'
        ],
        applications: {
            includeApplications: [
                '00000002-0000-0ff1-ce00-000000000000'
            ]
        },
        users: {
            includeGroups: ['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba']
        },
        locations: {
            includeLocations: [
                '198ad66e-87b3-4157-85a3-8a7b51794ee9'
            ]
        }
    },
    grantControls: {
        operator: 'OR',
        builtInControls: [
            'block'
        ]
    }
};

await client.api('/identity/conditionalAccess/policies')
    .post(conditionalAccessPolicy);

```