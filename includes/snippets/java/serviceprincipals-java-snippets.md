---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80877247eaa2758120bbe0334ff23ebd8c35f01a
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643929"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("{"ClaimsMappingPolicy": {
                "Version": 1,
                "IncludeBasicClaimSet": "true",
                "ClaimsSchema": [
                    {
                        "Source": "user",
                        "ID": "assignedroles",
                        "SamlClaimType": "https://aws.amazon.com/SAML/Attributes/Role"
                    },
                    {
                        "Source": "user",
                        "ID": "userprincipalname",
                        "SamlClaimType": "https://aws.amazon.com/SAML/Attributes/RoleSessionName"
                    },
                    {
                        "Source": "user",
                        "ID": "900",
                        "SamlClaimType": "https://aws.amazon.com/SAML/Attributes/SessionDuration"
                    },
                    {
                        "Source": "user",
                        "ID": "assignedroles",
                        "SamlClaimType": "appRoles"
                    },
                    {
                        "Source": "user",
                        "ID": "userprincipalname",
                        "SamlClaimType": "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier"
                    }
                ]
            }
        }");
claimsMappingPolicy.definition = definitionList;
claimsMappingPolicy.displayName = "AWS Claims policy";
claimsMappingPolicy.isOrganizationDefault = false;

graphClient.policies().claimsMappingPolicies()
    .buildRequest()
    .post(claimsMappingPolicy);

```