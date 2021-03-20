---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db11f11309b8a8974692514ff979e9506f56f6a8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949919"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("7679d9a4-2323-44cd-b5c2-673ec88d8b12");
appRoleAssignment.resourceId = UUID.fromString("076e8b57-bac8-49d7-9396-e3449b685055");
appRoleAssignment.appRoleId = UUID.fromString("00000000-0000-0000-0000-000000000000");

graphClient.groups("7679d9a4-2323-44cd-b5c2-673ec88d8b12").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```