---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88203669b28119db6045cefaae87d2c40883e19c
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
    definition: [
        '{\"ClaimsMappingPolicy\':{\'Version\':1,\'IncludeBasicClaimSet\':\'true\",\"ClaimsSchema\': [{\'Source\':\'user\",\"ID\':\'userprincipalname\",\"SamlClaimType\':\'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"},{\"Source\':\'user\",\"ID\':\'givenname\",\"SamlClaimType\':\'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname\"},{\"Source\':\'user\",\"ID\':\'displayname\",\"SamlClaimType\':\'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name\"},{\"Source\':\'user\",\"ID\':\'surname\",\"SamlClaimType\':\'http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname\"},{\"Source\':\'user\",\"ID\':\'userprincipalname\",\"SamlClaimType\':\'username\"}],\"ClaimsTransformation\':[{\'ID\':\'CreateTermsOfService\",\"TransformationMethod\':\'CreateStringClaim\",\"InputParameters\': [{\'ID\':\'value\",\"DataType\':\'string\", \"Value\':\'sandbox\"}],\"OutputClaims\':[{\'ClaimTypeReferenceId\':\'TOS\",\"TransformationClaimType\':\"createdClaim\"}]}]}}"
    ],
    displayName: 'Test1234'
};

await client.api('/policies/claimsMappingPolicies')
    .version('beta')
    .post(claimsMappingPolicy);

```