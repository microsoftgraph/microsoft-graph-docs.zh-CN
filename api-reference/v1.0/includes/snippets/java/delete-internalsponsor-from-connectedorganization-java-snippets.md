---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a12dd3122b296a52c80f7997e0a714537d7c6480
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336009"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{connectedOrganizationId}").internalSponsors("{id}").reference()
    .buildRequest()
    .delete();

```