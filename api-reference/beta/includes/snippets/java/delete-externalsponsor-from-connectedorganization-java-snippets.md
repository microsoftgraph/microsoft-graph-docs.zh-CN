---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0be20c7d5dbff8215c9bdd2196943a2c3f57ad0e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957806"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{connectedOrganizationId}").externalSponsors("{id}").reference()
    .buildRequest()
    .delete();

```