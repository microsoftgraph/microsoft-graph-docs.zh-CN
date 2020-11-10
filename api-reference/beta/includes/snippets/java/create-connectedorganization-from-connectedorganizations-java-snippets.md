---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51437ddc755371d08dd79327cd33b945e5dc6ef8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957588"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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