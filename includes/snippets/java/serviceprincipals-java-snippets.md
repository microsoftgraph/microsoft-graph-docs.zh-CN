---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b5d57be5cdb46bf0945cb24471253233bf06e98
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462566"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("{"ClaimsMappingPolicy":{"Version":1,"IncludeBasicClaimSet":"true", "ClaimsSchema": [{"Source":"user","ID":"assignedroles","SamlClaimType": "https://aws.amazon.com/SAML/Attributes/Role"}, {"Source":"user","ID":"userprincipalname","SamlClaimType": "https://aws.amazon.com/SAML/Attributes/RoleSessionName"}, {"Value":"900","SamlClaimType": "https://aws.amazon.com/SAML/Attributes/SessionDuration"}, {"Source":"user","ID":"assignedroles","SamlClaimType": "appRoles"}, {"Source":"user","ID":"userprincipalname","SamlClaimType": "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier"}]}}");
claimsMappingPolicy.definition = definitionList;
claimsMappingPolicy.displayName = "AWS Claims Policy";
claimsMappingPolicy.isOrganizationDefault = false;

graphClient.policies().claimsMappingPolicies()
    .buildRequest()
    .post(claimsMappingPolicy);

```