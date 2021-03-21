---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d520c0f3366779dae69f27c3f00746c64c99803
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962529"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("8fce32da-1246-437b-99cd-76d1d4677bd5");
appRoleAssignment.resourceId = UUID.fromString("9028d19c-26a9-4809-8e3f-20ff73e2d75e");
appRoleAssignment.appRoleId = UUID.fromString("ef7437e6-4f94-4a0a-a110-a439eb2aa8f7");

graphClient.servicePrincipals("9028d19c-26a9-4809-8e3f-20ff73e2d75e").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```