---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43482dc44ce69faeab076f87d2aed8f5179d4aaa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965032"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("principalId-value");
appRoleAssignment.resourceId = UUID.fromString("resourceId-value");
appRoleAssignment.appRoleId = UUID.fromString("appRoleId-value");

graphClient.servicePrincipals("{id}").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```