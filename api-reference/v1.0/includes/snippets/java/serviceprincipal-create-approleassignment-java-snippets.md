---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d33fa0074d499a745d0a3873b79b4aec41185159
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508045"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("9028d19c-26a9-4809-8e3f-20ff73e2d75e");
appRoleAssignment.resourceId = UUID.fromString("8fce32da-1246-437b-99cd-76d1d4677bd5");
appRoleAssignment.appRoleId = UUID.fromString("498476ce-e0fe-48b0-b801-37ba7e2685c6");

graphClient.servicePrincipals("9028d19c-26a9-4809-8e3f-20ff73e2d75e").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```