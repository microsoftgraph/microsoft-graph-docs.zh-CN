---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a029698e77e30a1bfd1f9e801799addf0739d2e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210308"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("8fce32da-1246-437b-99cd-76d1d4677bd5");
appRoleAssignment.resourceId = UUID.fromString("9028d19c-26a9-4809-8e3f-20ff73e2d75e");
appRoleAssignment.appRoleId = UUID.fromString("ef7437e6-4f94-4a0a-a110-a439eb2aa8f7");

graphClient.servicePrincipals("9028d19c-26a9-4809-8e3f-20ff73e2d75e").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```