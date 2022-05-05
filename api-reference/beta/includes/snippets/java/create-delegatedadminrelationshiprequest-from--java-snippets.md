---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 993b52fc7e2179d95072cdb3182756abd4b31654
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203466"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedAdminRelationshipRequest delegatedAdminRelationshipRequest = new DelegatedAdminRelationshipRequest();
delegatedAdminRelationshipRequest.action = DelegatedAdminRelationshipRequestAction.LOCK_FOR_APPROVAL;

graphClient.tenantRelationships().delegatedAdminRelationships("5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836").requests()
    .buildRequest()
    .post(delegatedAdminRelationshipRequest);

```