---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d16a4efbc9041c9152b801fd3979290eed0de0b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204107"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedAdminRelationshipOperation delegatedAdminRelationshipOperation = graphClient.tenantRelationships().delegatedAdminRelationships("5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836").operations("57e4479a-aafb-4d00-ab0f-8ce6027466cf")
    .buildRequest()
    .get();

```