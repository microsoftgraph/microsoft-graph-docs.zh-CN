---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6886beaf6859f6554430dfb71d8dcb70d628a231
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202526"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedAdminAccessAssignment delegatedAdminAccessAssignment = graphClient.tenantRelationships().delegatedAdminRelationships("72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409").accessAssignments("da9d6cf90-083a-47dc-ace2-1da98be3f344")
    .buildRequest()
    .get();

```