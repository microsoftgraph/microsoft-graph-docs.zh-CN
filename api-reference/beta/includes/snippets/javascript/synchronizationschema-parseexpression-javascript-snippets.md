---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbb173a2b0dd4dc314bec3476499cd1705787b069683f827103860193142fcfa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333649"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const parseExpressionResponse = {
    expression: 'Replace([preferredLanguage], \"-\", , , \"_\", ,  )',
    targetAttributeDefinition: null,
    testInputObject: {
        definition: null,
        properties:[
            { key: 'objectId', value : '66E4A8CC-1B7B-435E-95F8-F06CEA133828' },
            { key: 'IsSoftDeleted', value: 'false'},
            { key: 'accountEnabled', value: 'true'},
            { key: 'streetAddress', value: '1 Redmond Way'},
            { key: 'city', value: 'Redmond'},
            { key: 'state', value: 'WA'},
            { key: 'postalCode', value: '98052'},
            { key: 'country', value: 'USA'},
            { key: 'department', value: 'Sales'},
            { key: 'displayName', value: 'John Smith'},
            { key: 'extensionAttribute1', value: 'Sample 1'},
            { key: 'extensionAttribute2', value: 'Sample 2'},
            { key: 'extensionAttribute3', value: 'Sample 3'},
            { key: 'extensionAttribute4', value: 'Sample 4'},
            { key: 'extensionAttribute5', value: 'Sample 5'},
            { key: 'extensionAttribute6', value: 'Sample 6'},
            { key: 'extensionAttribute7', value: 'Sample 1'},
            { key: 'extensionAttribute8', value: 'Sample 1'},
            { key: 'extensionAttribute9', value: 'Sample 1'},
            { key: 'extensionAttribute10', value: 'Sample 1'},
            { key: 'extensionAttribute11', value: 'Sample 1'},
            { key: 'extensionAttribute12', value: 'Sample 1'},
            { key: 'extensionAttribute13', value: 'Sample 1'},
            { key: 'extensionAttribute14', value: 'Sample 1'},
            { key: 'extensionAttribute15', value: 'Sample 1'},
            { key: 'givenName', value: 'John'},
            { key: 'jobTitle', value: 'Finance manager'},
            { key: 'mail', value: 'johns@contoso.com'},
            { key: 'mailNickname', value: 'johns'},
            { key: 'manager', value: 'maxs@contoso.com'},
            { key: 'mobile', value: '425-555-0010'},
            { key: 'onPremisesSecurityIdentifier', value: '66E4A8CC-1B7B-435E-95F8-F06CEA133828'},
            { key: 'passwordProfile.password', value: ''},
            { key: 'physicalDeliveryOfficeName', value: 'Main Office'},
            { key: 'preferredLanguage', value: 'EN-US'},
            { key: 'proxyAddresses', value: ''},
            { key: 'surname', value: 'Smith'},
            { key: 'telephoneNumber', value: '425-555-0011'},
            { key: 'userPrincipalName', value: 'johns@contoso.com'},
            { key: 'appRoleAssignments', 'value@odata.type':'#Collection(String)', value: ['Default Assignment'] }
        ]
    }
};

await client.api('/servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression')
    .version('beta')
    .post(parseExpressionResponse);

```