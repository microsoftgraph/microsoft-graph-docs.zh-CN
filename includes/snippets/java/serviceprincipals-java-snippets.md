---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dc5cce6502adbaa037c00b262fceb5b87440258
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373570"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("{"ClaimsMappingPolicy":{"Version":1,"IncludeBasicClaimSet":"true", "ClaimsSchema": [{"Source":"user","ID":"assignedroles","SamlClaimType": "https://aws.amazon.com/SAML/Attributes/Role"}, {"Source":"user","ID":"userprincipalname","SamlClaimType": "https://aws.amazon.com/SAML/Attributes/RoleSessionName"}, {"Value":"900","SamlClaimType": "https://aws.amazon.com/SAML/Attributes/SessionDuration"}, {"Source":"user","ID":"assignedroles","SamlClaimType": "appRoles"}, {"Source":"user","ID":"userprincipalname","SamlClaimType": "https://aws.amazon.com/SAML/Attributes/nameidentifier"}]}}");
claimsMappingPolicy.definition = definitionList;
claimsMappingPolicy.displayName = "AWS Claims Policy";
claimsMappingPolicy.isOrganizationDefault = false;

graphClient.policies().claimsMappingPolicies()
    .buildRequest()
    .post(claimsMappingPolicy);

```