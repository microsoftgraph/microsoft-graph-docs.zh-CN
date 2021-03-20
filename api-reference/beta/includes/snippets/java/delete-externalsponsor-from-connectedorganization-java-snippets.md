---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5131efdb22e0478f8446e37976d764be6fb86a81
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970301"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{connectedOrganizationId}").externalSponsors("{id}").reference()
    .buildRequest()
    .delete();

```