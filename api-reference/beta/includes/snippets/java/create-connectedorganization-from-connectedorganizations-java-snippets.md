---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a42c19812776a393ec1a92d7786e68c60c01cac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969613"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectedOrganization connectedOrganization = new ConnectedOrganization();
connectedOrganization.displayName = "Connected organization name";
connectedOrganization.description = "Connected organization description";
LinkedList<IdentitySource> identitySourcesList = new LinkedList<IdentitySource>();
DomainIdentitySource identitySources = new DomainIdentitySource();
identitySources.domainName = "example.com";
identitySources.displayName = "example.com";
identitySourcesList.add(identitySources);
connectedOrganization.identitySources = identitySourcesList;
connectedOrganization.state = ConnectedOrganizationState.PROPOSED;

graphClient.identityGovernance().entitlementManagement().connectedOrganizations()
    .buildRequest()
    .post(connectedOrganization);

```