---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ee0249fab276763671bb1859e84e9947626821ac48cadde9eebbd3dcba01ab9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161574"
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