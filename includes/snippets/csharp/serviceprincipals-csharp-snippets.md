---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8589604ff8262b514b39edf3fa7e0d021cb2e367
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643930"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicy = new ClaimsMappingPolicy
{
    Definition = new List<String>()
    {
        "{\"ClaimsMappingPolicy\": {\r\n                \"Version\": 1,\r\n                \"IncludeBasicClaimSet\": \"true\",\r\n                \"ClaimsSchema\": [\r\n                    {\r\n                        \"Source\": \"user\",\r\n                        \"ID\": \"assignedroles\",\r\n                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"\r\n                    },\r\n                    {\r\n                        \"Source\": \"user\",\r\n                        \"ID\": \"userprincipalname\",\r\n                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"\r\n                    },\r\n                    {\r\n                        \"Source\": \"user\",\r\n                        \"ID\": \"900\",\r\n                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"\r\n                    },\r\n                    {\r\n                        \"Source\": \"user\",\r\n                        \"ID\": \"assignedroles\",\r\n                        \"SamlClaimType\": \"appRoles\"\r\n                    },\r\n                    {\r\n                        \"Source\": \"user\",\r\n                        \"ID\": \"userprincipalname\",\r\n                        \"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"\r\n                    }\r\n                ]\r\n            }\r\n        }"
    },
    DisplayName = "AWS Claims policy",
    IsOrganizationDefault = false
};

await graphClient.Policies.ClaimsMappingPolicies
    .Request()
    .AddAsync(claimsMappingPolicy);

```