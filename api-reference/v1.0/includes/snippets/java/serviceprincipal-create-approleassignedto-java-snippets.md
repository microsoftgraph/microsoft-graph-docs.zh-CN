---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6223b44bb09e22e8528fcd073d0dfb76b03b055a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970252"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("33ad69f9-da99-4bed-acd0-3f24235cb296");
appRoleAssignment.resourceId = UUID.fromString("9028d19c-26a9-4809-8e3f-20ff73e2d75e");
appRoleAssignment.appRoleId = UUID.fromString("ef7437e6-4f94-4a0a-a110-a439eb2aa8f7");

graphClient.servicePrincipals("9028d19c-26a9-4809-8e3f-20ff73e2d75e").appRoleAssignedTo()
    .buildRequest()
    .post(appRoleAssignment);

```